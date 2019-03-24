# Renew SSL Certificate


```sh
# SSH to the server you like to generate and install certificate
ssh root@example.com
cd ~

# Create a directory for generating and keeping private key, CSR file 
mkdir -p keys/example.com

cd keys/example.com

# Generate private key and csr file using openssl
openssl req -newkey rsa:2048 -nodes -keyout example.com.key -out example.com.csr
cat example.com.csr

cat example.com.csr

# Copy the contents of CSR and paste it in your SSL provider like (GoDaddy, Comodo)
# If you like to generate from certificate, checkout https://letsencrypt.org/
```
