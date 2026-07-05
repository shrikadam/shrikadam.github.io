Here is your complete, end-to-end cheat sheet for publishing a new blog post with an image. Keep this handy for whenever you want to update your site!

### 📂 Step 1: Organize Your Image

Before you write a single word, get your media organized so your repository stays clean.

1. Navigate to your `assets/images/posts/` folder.
2. Create a new folder specifically for this post. Let's call it `my-post`.
3. Drop your image into that new folder (e.g., `image.jpg`).
* *Path:* `assets/images/posts/my-post/image.jpg`

### 📄 Step 2: Create the Markdown File

Jekyll requires a very strict naming convention for posts so it knows how to date them automatically.

1. Go into your `_posts/` folder.
2. Create a new file named with today's date and your URL slug: `2026-07-05-my-post.md`.

### ✍️ Step 3: Write the Front Matter

Open your new `.md` file. At the very top, you must tell Jekyll what layout to use and what the title is. Paste this:

```markdown
---
layout: post
title: "My Second Post: Hardware Integration"
subtitle: "Wiring the new robotic arm and debugging the servos."
---
```

### 🖼️ Step 4: Write the Content & Insert the Image

Below the second `---`, write your blog post using standard Markdown.

To insert the image you saved in Step 1, use the Markdown image syntax. **Make sure you include the leading forward slash (`/`)** so Jekyll knows to look from the root of your website:

```markdown
It took a few tries, but the new robotic arm is finally wired up and responding to the controller.

Here is a look at the final hardware setup:

![A custom 3D printed robotic arm](/assets/images/posts/my-post/image.jpg)

The next step will be writing the Python script to control the kinematics. Here is a sneak peek:

```python
def move_to_target(x, y, z):
    # Kinematics logic goes here
    pass
```


### 💻 Step 5: Preview Locally
Don't push it to the world until you know it looks perfect.
1. Open your terminal and navigate to your `shrikadam.github.io` folder.
2. Run your local server:
   ```bash
   bundle exec jekyll serve
   ```

3. Open your browser to `http://127.0.0.1:4000`.
4. Check your homepage—you will see "My Second Post" automatically added to the top of the Blog list! Click it to make sure your image loaded correctly and the code highlighting looks good.

### 🚀 Step 6: Publish to GitHub

Once you are happy with the local preview, stop the server (press `Ctrl + C` in the terminal) and push your changes to GitHub.

```bash
git add .
git commit -m "Added new blog post with image"
git push origin main
```

Wait about 60 seconds, refresh your live `shrikadam.github.io` website, and your new post will be live for everyone to read.