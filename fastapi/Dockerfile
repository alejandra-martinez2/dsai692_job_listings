# Use python:3.13-slim as a base image 
FROM python:3.13-slim

# Set  as a working directory
WORKDIR /fastapi

# Copy environment.yml
COPY * ./

# Install required packages/libs
RUN pip install -r requirements.txt

# #xpose port 8000
EXPOSE 8000

# Run streamlit
CMD ["fastapi", "run", "extract_save_data.py", "--port", "8000"]