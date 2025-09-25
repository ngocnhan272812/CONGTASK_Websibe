# Placeholder Grid System Documentation

## 📋 Overview
CSS Grid system được thêm vào từ line 154 trong `style.css` để quản lý placeholder images trong tương lai.

## 🎯 Features

### ✅ **Responsive Grid Layout**
- **Auto-fit columns**: Minimum 300px width
- **Flexible gaps**: 2rem default, responsive
- **Mobile optimization**: 2 columns → 1 column

### ✅ **Interactive Effects**
- **Hover animations**: Transform translateY(-5px)
- **Shadow transitions**: Smooth box-shadow changes
- **Visual feedback**: Better user experience

### ✅ **Image Management**
- **Consistent sizing**: 250px height (200px on mobile)
- **Object-fit cover**: Proper image scaling
- **Border radius**: 12px for modern look
- **Background fallback**: #f0f0f0 color

### ✅ **Caption System**
- **Title support**: h4 styling
- **Description area**: p tag for details
- **Centered layout**: Professional appearance

## 🔧 Usage

### Basic Implementation:
```html
<div class="placeholder-grid">
    <div class="placeholder-item">
        <img src="placeholder-url" alt="Description" />
        <div class="placeholder-caption">
            <h4>Image Title</h4>
            <p>Image description</p>
        </div>
    </div>
    <!-- More items... -->
</div>
```

### CSS Classes:
- `.placeholder-grid` - Main container
- `.placeholder-item` - Individual image container
- `.placeholder-caption` - Text area below image

## 📱 Responsive Breakpoints

### Desktop (>768px):
- Auto-fit columns (minimum 300px)
- 2rem gap between items
- 250px image height

### Tablet (≤768px):
- 2 columns fixed
- 1.5rem gap
- 250px image height

### Mobile (≤480px):
- 1 column
- 1rem gap
- 200px image height

## 🎨 Styling Options

### Hover State:
```css
.placeholder-item:hover {
    transform: translateY(-5px);
    box-shadow: 0 15px 30px rgba(0,0,0,0.15);
}
```

### Image Styling:
```css
.placeholder-item img {
    width: 100%;
    height: 250px;
    object-fit: cover;
    border-radius: 12px;
}
```

## 📂 File References
- **CSS**: Line 154+ in `css/style.css`
- **Example**: `placeholder-grid-example.html`
- **Implementation**: Ready để thêm vào bất kỳ section nào

## 💡 Use Cases
- Portfolio galleries
- Team member photos
- Client logos grid
- Product showcases
- Before/after images
- Case study visuals

## 🚀 Future Enhancements
- [ ] Lightbox integration
- [ ] Image lazy loading
- [ ] Filter/sort functionality
- [ ] Masonry layout option
- [ ] Video placeholder support
