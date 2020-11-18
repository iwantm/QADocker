# Use Python Image
FROM python:3.7
WORKDIR /app
# Install apt dependencies
RUN pip install Flask
# Copy contents into image
COPY app.py .
# Run pip dependencies
 
# Expose the correct port
EXPOSE 5000
# Create an entrypoint
ENTRYPOINT ["python","app.py"]
