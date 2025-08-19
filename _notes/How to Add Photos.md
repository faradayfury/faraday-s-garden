---
title: How to Add Photos to Your Digital Garden
date: 2024-12-19
---

## Quick Photo Upload Workflow

#### Step 1: Prepare Your Photos

- **Format**: Save as `.jpg`, `.jpeg`, or `.png`
- **Size**: Optimize for web (recommended max 1500px width)
- **File Size**: Keep under 1MB each for good loading performance
- **Naming**: Use descriptive, web-safe names (e.g., `tokyo-street-2024.jpg`)

#### Step 2: Add Photo Files

1. Navigate to `/assets/photos/` in your file system
2. Copy your photo files into this folder
3. Note the exact filename you used

#### Step 3: Update Photo Data

1. Open `/_data/photos.yml` in any text editor (or through Obsidian)
2. Add a new entry at the end of the list:

```yaml
- filename: "your-photo.jpg"
  alt: "Brief description for screen readers"
  caption: "Photo title or caption"
  location: "Where it was taken"
  date: "YYYY-MM"
```

#### Step 4: Build Your Site

- Run your Jekyll build process
- Photos will automatically appear on the homepage

## From Obsidian

#### Adding Photos via Obsidian

1. **Copy photos** to the `/assets/photos/` folder (accessible from your file system)
2. **Edit the data file**: Open `/_data/photos.yml` in Obsidian as a regular file
3. **Add your entry** following the format above
4. **Save and rebuild** your Jekyll site

## Example Entry

```yaml
- filename: "sunset-barcelona-2024.jpg"
  alt: "Golden sunset over Barcelona rooftops"
  caption: "Evening light in El Born neighborhood"
  location: "Barcelona, Spain"
  date: "2024-01"
```

## Tips

#### Photo Organization

- Keep a consistent naming convention
- Include location/date in filenames when possible
- Organize by year or theme if you have many photos

#### Technical Notes

- Photos display in the order they appear in `photos.yml`
- The grid shows up to 16 photos, with placeholders filling remaining spaces
- All fields except `filename` and `alt` are optional
- Photos get lazy loading for better performance
