# Generating Snake GIF/SVG to display in Profile README.md

- Refer to this Blog for Generating the Snake Gif which eats the Commits we did in our account.
https://dev.to/mishmanners/how-to-enable-github-actions-on-your-profile-readme-for-a-contribution-graph-4l66 
- Youtube references: 
https://www.youtube.com/watch?v=7FHiew0_NLQ
https://www.youtube.com/watch?v=pkY18HTfeL8

# Steps:
- Create GitHub Actions yml file first. Take the code snippet from above blog or Youtubers GitHUb Account. 
  Make sure to change the Username and branch as main in the "push the changes" section of yml file.
  You can also add one more condition if you want workflow to trigger on every push in the same yml file.
  
  **Note1:** Since you are using GitHub token you need to pass PAT in the repo secrets. ( Generate PAT and then go to Repo Setting --> Secrets and Variables --> Actions --> Add PAT)
            Then Repo Setting --> Actions --> General --> Workflow permissions --> Enable read and write permissions
            Then Repo Settings --> Pages --> Build and Deployment --> Branch --> Output --> Save. You can change this later.
   **Note2:** This GitHub Pages will publish a site based on the branch you are selecting. Since our Readme page is in Main,
              and you gave branch as main then a site will be published in 2 mins.

- Then execute the workflow once. So that new output branch will be created and GIF/SVG file will be added there.
- You have to use the location of any one file in the Readme file. 
