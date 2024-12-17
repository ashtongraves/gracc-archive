FROM opensciencegrid/software-base:23-el9-release
COPY src/graccarchive/* /app/
WORKDIR /app
RUN ["dnf", "install", "-y", "pip"]
RUN ["pip", "install", "-r", "requirements.txt"]
ENTRYPOINT ["python3", "graccarchive.py"]