simple Conversation app using Discovery for Long tail questions

# Links

https://github.com/watson-developer-cloud/conversation-with-discovery

https://github.com/watson-developer-cloud/conversation-simple

#  .env file
# Environment variables
WORKSPACE_ID= 
CONVERSATION_USERNAME= 
CONVERSATION_PASSWORD= 

DISCOVERY_USERNAME= 
DISCOVERY_PASSWORD= 
ENVIRONMENT_ID=
COLLECTION_ID= 

# manifest.yml file
---
applications:
- name: chemical-demo-json
  command: npm start
  path: .
  memory: 256M
  instances: 1
  services:
  - Conversation-ce
  - discovery-service
  env:
    NPM_CONFIG_PRODUCTION: false


