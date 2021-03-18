# url-redirector
This is a simple docker based URL redirector. It listens on port 80 and redirect all the traffic to this port to a 
designated website. By default it uses http redirect `301 moved permanently`. 

Depending on the use cases, `303` might be more precise when sites are running on 
the particular server while only redirecting some ports away, or some pages away. 

### How to use
Run the docker container
```bash
docker-compose up -d
```

The -d option keeps the container running in the background. The restart policy is set to 
`always`, it should be restart-proof. 