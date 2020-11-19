# Use Python Image
FROM python:3.7
# Install apt dependencies
RUN pip install Flask
# Copy contents into image
COPY app.py .
# Run pip dependencies
EXPOSE 5000
# Expose the correct port
ENTRYPOINT ["python", "app.py"]
# Create an entrypoint

