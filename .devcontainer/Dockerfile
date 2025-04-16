# Use Ubuntu as the base image
FROM ubuntu:24.10

# Avoid prompts from apt
ENV DEBIAN_FRONTEND=noninteractive

# Update the package lists and install only necessary packages
RUN apt-get update && apt-get install -y --no-install-recommends \
    build-essential \
    python3-dev \
    python3-pip \
    python3-setuptools \
    python3-wheel \
    python3-cffi \
    libcairo2 \
    libpango-1.0-0 \
    libpangocairo-1.0-0 \
    libgdk-pixbuf2.0-0 \
    libffi-dev \
    shared-mime-info \
    libglib2.0-dev \
    curl \
    ca-certificates \
    python3-full \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

# Install Node.js
RUN curl -fsSL https://deb.nodesource.com/setup_lts.x | bash - && \
    apt-get update && \
    apt-get install -y nodejs && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*

# Verify Node.js installation
RUN node --version && npm --version

# Set up virtual environment
RUN python3 -m venv /opt/venv
ENV PATH="/opt/venv/bin:$PATH"

# Set the working directory
WORKDIR /app


# FOR THE VPS
# Then copy your requirements file
# COPY requirements.txt .

# Set up virtual environment
RUN python3 -m venv /opt/venv
ENV PATH="/opt/venv/bin:$PATH"

# # Now install requirements
# RUN pip install -r requirements.txt

# # Finally copy the rest of your application
# COPY . .





# Command to run when the container starts
# CMD ["gunicorn", "app:app", "--bind", "0.0.0.0:5000"]

# === README ===
# Why use `apk` here?
# - This Dockerfile uses `alpine:latest` as the base image, which is based on Alpine Linux.
# - Alpine Linux uses `apk` as its package manager, not `apt-get`.
# - `apk` is lightweight and designed for Alpine's minimalistic environment.
#
# When to use `apt-get`:
# - If you switch to a Debian/Ubuntu-based image (e.g., `ubuntu:slim`), you must use `apt-get` instead of `apk`.
# - Debian/Ubuntu uses `glibc`, which is more compatible with some software but results in larger image sizes.
#
# When to use `apk`:
# - When using Alpine-based images for their extremely small size (~5 MB).
# - If your application is compatible with Alpine's `musl libc` and you prioritize minimalism.
#
# Choose the base image based on your needs:
# - For smallest size: Use Alpine (`apk`).
# - For compatibility: Use Ubuntu Slim (`apt-get`).
