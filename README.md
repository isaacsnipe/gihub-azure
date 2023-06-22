# web-app
# new commit
# commit
# Done
/**
 - name: Azure Login
        uses: azure/login@v1
        with:
          creds: ${{ secrets.AZURE_CREDENTIALS }}
    
      - name: Azure WebApp Deployment
        uses: Azure/webapps-deploy@v2
        with:
        # Name of the Azure Web App
          app-name: '${{env.AZURE_WEB_APP}}'
        # Applies to Web App Containers only: Specify the fully qualified container image(s) name. For example, 'myregistry.azurecr.io/nginx:latest' or 'python:3.7.2-alpine/'. For multi-container scenario multiple container image names can be provided (multi-line separated)
          images: '${{secrets.DOCKER_LOGIN}}/${{env.DOCKER_IMAGE_NAME}}:latest'
      
**?
