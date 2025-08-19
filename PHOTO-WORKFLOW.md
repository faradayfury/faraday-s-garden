# 📸 Photo Upload Workflow

Your photography section is now set up with a data-driven system that makes adding photos simple and organized.

## How It Works

**File Structure:**

```
/assets/photos/          # Your photo files go here
/_data/photos.yml        # Photo metadata and organization
```

**Display System:**

- Photos are dynamically generated from the data file
- Maintains your responsive grid layout
- Shows up to 16 photos with placeholders for remaining slots
- Includes lazy loading for performance

## Adding New Photos

### 1. Add Photo Files

Copy your optimized photos to `/assets/photos/`:

- **Formats**: JPG, JPEG, PNG
- **Size**: Max 1500px width recommended
- **File Size**: Under 1MB each for good performance

### 2. Update Photo Data

Edit `/_data/photos.yml` and add entries like:

```yaml
- filename: "your-photo.jpg"
  alt: "Description for accessibility"
  caption: "Photo title/caption"
  location: "Where taken"
  date: "YYYY-MM"
```

### 3. Rebuild Site

Run your Jekyll build - photos appear automatically!

## Features

✅ **Data-driven**: Easy to manage and reorganize  
✅ **Responsive**: Works on all device sizes  
✅ **Accessible**: Alt text and proper markup  
✅ **Performance**: Lazy loading and optimized display  
✅ **Flexible**: Add metadata like captions, locations, dates  
✅ **Obsidian Compatible**: Edit data files directly in your vault

## Current Setup

You have 6 sample entries in your data file to get started. Replace these with your actual photos by:

1. Adding real photo files to `/assets/photos/`
2. Updating the entries in `/_data/photos.yml` with your photo details

Your photography section will automatically reflect any changes after rebuilding the site!

## Integration with Obsidian

Since your `_data` folder is part of your project (not in the `_notes` vault), you can:

- Edit `photos.yml` in any text editor
- Or access it through the parent folder when working in Obsidian
- The workflow remains simple and doesn't interfere with your note-taking

Ready to showcase your photography! 🚀
