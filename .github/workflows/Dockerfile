FROM python:3.10
WORKDIR /app
COPY . .
RUN pip install -r requirements.txt
CMD ["python", "app.py"]

gcloud builds submit --tag us-central1-docker.pkg.dev/shyamproject-481517/agents/devops-agent
gcloud run deploy devops-agent --image us-central1-docker.pkg.dev/shyamproject-481517/agents/devops-agent --allow-unauthenticated
