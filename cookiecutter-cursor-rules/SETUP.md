# Setting Up Your Cookiecutter Template on GitHub

Follow these steps to host your cookiecutter template on GitHub so it can be used with the command:
```
cookiecutter gh:yourusername/cursor-rules-template --checkout template
```

## 1. Create a GitHub Repository

1. Go to [GitHub](https://github.com) and sign in to your account
2. Click the "+" icon in the top right corner and select "New repository"
3. Name your repository `cursor-rules-template` (or whatever name you prefer)
4. Add a description (optional)
5. Choose public visibility (so others can use your template)
6. Initialize with a README (optional, since we already have one)
7. Click "Create repository"

## 2. Push Your Template to GitHub

After creating the repository, push your template to GitHub:

```bash
# Navigate to your template directory
cd cookiecutter-cursor-rules

# Initialize git repository
git init

# Add all files
git add .

# Commit the files
git commit -m "Initial commit of cookiecutter template"

# Add your GitHub repository as remote
git remote add origin https://github.com/yourusername/cursor-rules-template.git

# Push to GitHub
git push -u origin main
```

## 3. Create a Template Branch

To support the `--checkout template` option, create a branch named "template":

```bash
# Create and switch to a new branch named "template"
git checkout -b template

# Push the template branch to GitHub
git push -u origin template
```

## 4. Using Your Template

Now others (or you) can use your template with:

```bash
cookiecutter gh:yourusername/cursor-rules-template --checkout template
```

Replace `yourusername` with your actual GitHub username.

## 5. Updating Your Template

When you want to update your template:

1. Make your changes
2. Commit them
3. Push to the template branch:

```bash
git add .
git commit -m "Update template with new features"
git push origin template
```

## 6. Documentation

Make sure to update the README.md with any changes to your template's features or usage instructions. 