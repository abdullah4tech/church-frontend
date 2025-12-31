# Gallery Image Organization Guide

This folder contains all gallery images organized by year and month for easy management.

## Folder Structure

```
images/gallery/
├── 2025/
│   ├── december/
│   ├── november/
│   ├── october/
│   └── [other months]/
├── 2024/
│   ├── august/
│   ├── april/
│   ├── january/
│   └── [other months]/
└── 2023/
    └── [months]/
```

## How to Add New Gallery Images

1. **Create a month folder** if it doesn't exist:
   - Navigate to the appropriate year folder (e.g., `2025/`)
   - Create a new folder with the month name in lowercase (e.g., `september/`)

2. **Add your images**:
   - Copy your event photos into the appropriate month folder
   - Use descriptive filenames (e.g., `christmas-service-01.jpg`, `youth-conference-worship.jpg`)

3. **Update gallery.html**:
   - Open `gallery.html` in your editor
   - Find the timeline section
   - Add a new timeline-item for your event following this template:

```html
<div class="timeline-item" data-year="2025">
  <div class="timeline-header">
    <div class="timeline-date">Sep 2025</div>
    <div class="timeline-title">
      <h3>Your Event Name</h3>
      <p>Short event description</p>
    </div>
  </div>
  
  <div class="event-description">
    <p>
      Detailed description of what happened during the event...
    </p>
  </div>

  <div class="gallery-grid">
    <div class="gallery-item">
      <img src="images/gallery/2025/september/image-01.jpg" alt="Description" />
      <div class="gallery-item-overlay">
        <p>Image Caption</p>
      </div>
    </div>
    <!-- Add more gallery-item divs for each image -->
  </div>
</div>
```

## Image Specifications

- **Format**: JPG or PNG
- **Recommended size**: 1200px wide (will be automatically resized)
- **Aspect ratio**: 4:3 works best (e.g., 1200x900px)
- **File size**: Keep under 500KB per image for fast loading

## Tips for Best Results

1. **Naming Convention**: Use descriptive names with hyphens
   - Good: `easter-baptism-ceremony.jpg`
   - Avoid: `IMG_1234.jpg`

2. **Image Quality**: Use high-quality photos but compress them for web
   - Tools: TinyPNG.com, ImageOptim, or Photoshop "Save for Web"

3. **Event Organization**: 
   - Group related photos together
   - Put your best/main photo first in the gallery grid
   - Include 3-6 images per event for best display

4. **Timeline Order**: 
   - Events are displayed in chronological order (newest first)
   - Make sure to add new events at the top of the timeline section

## Example Events to Include

- Monthly Services
- Special Celebrations (Christmas, Easter, Thanksgiving)
- Church Anniversaries
- Conferences and Seminars
- Youth Events
- Baptisms
- Community Outreach
- Fundraisers
- Bible Study Groups
- Fellowship Meals

## Filter System

The gallery includes a year filter at the top. Make sure to:
- Set the correct `data-year` attribute on each timeline-item
- Add new year buttons to the filter section if needed

## Need Help?

If you need assistance updating the gallery or have questions about image organization, feel free to reach out!
