FROM debian:latest

# Set non-interactive mode for apt
ENV DEBIAN_FRONTEND=noninteractive

# Install necessary dependencies and TeX Live with XeLaTeX
RUN apt-get update && apt-get install -y \
    texlive-xetex \
    texlive-fonts-recommended \
    texlive-fonts-extra \
    texlive-latex-extra \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*
    
# Default command
CMD ["xelatex", "--version"]
