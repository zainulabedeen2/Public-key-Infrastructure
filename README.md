#Public-Key-Infrastructure
 ###### Name zain	ul abedeen
	 Tittle: Public-Key-Infrastructure
   Instruction: https://seedsecuritylabs.org/Labs_16.04/PDF/Crypto_PKI.pdf
   #### Task 1
   Copy the configuration file into current directory:
   
      cp /usr/lib/ssl/openssl.cnf ./openssl.cnf
      
  create new sub-directories and files according to what it specifies in its [ CA_default ] section:
  
              dir = ./demoCA # Where everything is kept
             certs = $dir/certs # Where the issued certs are kept
             crl_dir = $dir/crl # Where the issued crl are kept
             new_certs_dir = $dir/newcerts # default place for new certs.
             database = $dir/index.txt # database index file.
             serial = $dir/serial # The current serial number
             Simply create an empty file for index.txt, put a single number in string format in serial:
 Simply create an empty file for index.txt, put a single number in string format in serial:

            cp "/usr/lib/ssl/openssl.cnf" "/home/seed/PKI/"
            mkdir demoWK
            cd demoWK
             mkdir certs crl newcerts
             echo 1000 > serial
             gedit index.txt
  Start to generate the self-signed certificate for the CA:

            # return to the parent directory
            # cd ..
            openssl req -new -x509 -keyout ca.key -out ca.crt -config openssl.cnf 
When asked to type PEM pass phrase, remember the password you typed (e.g. I use seeddes). It will then ask you to fill in some information, you can skip it by Enter, except for those required by policy_match.

            Generating a 2048 bit RSA private key
              ...................+++
             .............................................................................+++
            writing new private key to 'ca.key'
            Enter PEM pass phrase:
            Verifying - Enter PEM pass phrase:
             -----
            You are about to be asked to enter information that will be incorporated
            into your certificate request.
            What you are about to enter is what is called a Distinguished Name or a DN.
            There are quite a few fields but you can leave some blank
            For some fields there will be a default value,
            If you enter '.', the field will be left blank.
            
            Country Name (2 letter code) [AU]:PK
            State or Province Name (full name) [Some-State]:sahiwal
             Locality Name (eg, city) []:swl
             Organization Name (eg, company) [Internet Widgits Pty Ltd]:UOS
             Organizational Unit Name (eg, section) []:UOSahiwal
             Common Name (e.g. server FQDN or YOUR name) []:Asad Ali
             Email Address []:www.zainsajid158@gmail.com
      
      
     
      
      
     
https://github.com/zainulabedeen2/Public-key-Infrastructure/blob/main/task1.png

https://github.com/zainulabedeen2/Public-key-Infrastructure/blob/main/task2a.png

https://github.com/zainulabedeen2/Public-key-Infrastructure/blob/main/task2b.png

https://github.com/zainulabedeen2/Public-key-Infrastructure/blob/main/task2b.png

https://github.com/zainulabedeen2/Public-key-Infrastructure/blob/main/task2c.png

https://github.com/zainulabedeen2/Public-key-Infrastructure/blob/main/task2d.png

https://github.com/zainulabedeen2/Public-key-Infrastructure/blob/main/task2e.png

https://github.com/zainulabedeen2/Public-key-Infrastructure/blob/main/task2f.png

https://github.com/zainulabedeen2/Public-key-Infrastructure/blob/main/task3.png

https://github.com/zainulabedeen2/Public-key-Infrastructure/blob/main/task3a.png

https://github.com/zainulabedeen2/Public-key-Infrastructure/blob/main/task3b.png

https://github.com/zainulabedeen2/Public-key-Infrastructure/blob/main/task3c.png

https://github.com/zainulabedeen2/Public-key-Infrastructure/blob/main/task3d.png

https://github.com/zainulabedeen2/Public-key-Infrastructure/blob/main/task3e.png

https://github.com/zainulabedeen2/Public-key-Infrastructure/blob/main/task3f.png

https://github.com/zainulabedeen2/Public-key-Infrastructure/blob/main/task3g.png

https://github.com/zainulabedeen2/Public-key-Infrastructure/blob/main/task4a.png

https://github.com/zainulabedeen2/Public-key-Infrastructure/blob/main/task4b.png

https://github.com/zainulabedeen2/Public-key-Infrastructure/blob/main/task4c.png

https://github.com/zainulabedeen2/Public-key-Infrastructure/blob/main/task4d.png

https://github.com/zainulabedeen2/Public-key-Infrastructure/blob/main/task4e.png

https://github.com/zainulabedeen2/Public-key-Infrastructure/blob/main/task4f.png

https://github.com/zainulabedeen2/Public-key-Infrastructure/blob/main/task4g.png

https://github.com/zainulabedeen2/Public-key-Infrastructure/blob/main/task5a.png

https://github.com/zainulabedeen2/Public-key-Infrastructure/blob/main/task5b.png
