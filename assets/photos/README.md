# 📸 Photography Folder

This folder contains all the photos displayed on your website's photography section.

## How to Add New Photos

### Step 1: Add Photo Files

- Copy your `.jpg`, `.jpeg`, or `.png` files to this folder
- **Recommended**: Use web-optimized images (under 1MB each)
- **Naming**: Use descriptive, web-safe filenames (e.g., `tokyo-street-night.jpg`)

### Step 2: Update Photo Data

- Open `/_data/photos.yml`
- Add a new entry for your photo following the format:

```yml
- filename: "your-photo.jpg"
  alt: "Brief description for accessibility"
  caption: "Photo title/caption"
  location: "Where it was taken"
  date: "YYYY-MM"
```

### Step 3: Rebuild Site

Your photo will automatically appear on the homepage after Jekyll rebuilds.

## Photo Guidelines

**Image Specs:**

- **Format**: JPG, JPEG, or PNG
- **Size**: Recommended max 1500px width
- **Quality**: Web-optimized (balance quality/file size)
- **File Size**: Under 1MB per image for good performance

**Naming Convention:**

- Use lowercase, hyphen-separated names
- Avoid spaces and special characters
- Example: `mountain-sunrise-alps.jpg`

## Current Photos

The photos displayed on your site are managed through the `/_data/photos.yml` file.
