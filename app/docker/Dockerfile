# Base image
FROM python:3.7

# Create all the directories
RUN mkdir /app
RUN mkdir /app/pipeline
RUN mkdir /app/pipeline/model
RUN mkdir /app/pipeline/preprocessing
RUN mkdir /app/pipeline/utils

# Copy the different files
COPY app/pipeline/model/model.py /app/pipeline/model/model.py
COPY app/pipeline/preprocessing/preprocessing.py /app/pipeline/preprocessing/preprocessing.py
COPY app/pipeline/utils/utils.py /app/pipeline/utils/utils.py

# Run the model file
WORKDIR /app/pipeline

CMD ["python", "model/model.py"]
