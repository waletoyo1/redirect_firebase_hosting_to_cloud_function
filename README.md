# redirect_firebase_hosting_to_cloud_function
How to redirect a firebase hosting site to a cloud function url

1. add "site:"site_name" to firebase.json file
2. add "rewrites": [
  {
    "source": "**",
    "function": "function_name"
  }
] to firebase.json file

3. Make sure you do not have any index.html file in the public folder

4. Run firebase deploy --only hosting:site_name
