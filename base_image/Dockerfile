# Step 1/3
# 
FROM debian

# Step 2/3
RUN apt-get update && apt-get install -y lighttpd && rm -rf /var/lib/apt/lists/*

# Step 3/3
ENTRYPOINT lighttpd -D -f /etc/lighttpd/lighttpd.conf