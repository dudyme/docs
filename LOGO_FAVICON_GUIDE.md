# Logo and Favicon Setup Guide

This guide provides specifications and requirements for creating logo and favicon files for the Call24x7 documentation.

## Logo Files

### File Locations

- **Dark logo**: `/logo/dark.svg` - Used on light backgrounds
- **Light logo**: `/logo/light.svg` - Used on dark backgrounds

### Specifications

#### Dark Logo (`/logo/dark.svg`)

- **Purpose**: Displayed on light/white backgrounds
- **Format**: SVG (vector format preferred)
- **Size**: Optimized for documentation header (typically 200-300px width)
- **File size**: Maximum 50KB
- **Colors**: Should be visible on white/light backgrounds
- **Design**: Human head with circuitry and telephone receiver (as described)

#### Light Logo (`/logo/light.svg`)

- **Purpose**: Displayed on dark backgrounds
- **Format**: SVG (vector format preferred)
- **Size**: Optimized for documentation header (typically 200-300px width)
- **File size**: Maximum 50KB
- **Colors**: Should be visible on dark backgrounds
- **Design**: Same design as dark logo but with inverted/light colors

### Design Requirements

Based on the provided design description:

- **Primary element**: Human head profile (left-facing)
- **Circuitry elements**: White lines and nodes representing technology/brain
- **Telephone receiver**: Integrated within the head, positioned near the ear area
- **Style**: Minimalist, two-tone aesthetic
- **Brand colors**: Should align with Call24x7 brand colors:
  - Primary: `#0D9373`
  - Light: `#07C983`

### Contrast Requirements

- **Dark logo**: Must have sufficient contrast on white backgrounds (WCAG AA minimum)
- **Light logo**: Must have sufficient contrast on dark backgrounds (WCAG AA minimum)

## Favicon

### File Location

- **Favicon**: `/favicon.svg` - Used as the browser tab icon

### Specifications

- **Format**: SVG (preferred) or PNG with multiple sizes
- **Size**: Must be recognizable at small sizes (16x16, 32x32, 48x48, 192x192)
- **Design**: Simplified version of the logo or icon
- **Colors**: Should align with brand colors (`#0D9373`, `#07C983`)

### SVG Favicon (Recommended)

SVG format is preferred because:
- Scales to any size without quality loss
- Single file for all sizes
- Smaller file size
- Better browser support

### PNG Favicon (Alternative)

If using PNG, provide multiple sizes:
- `16x16` - Browser tab icon
- `32x32` - Browser tab icon (high DPI)
- `48x48` - Browser bookmark icon
- `192x192` - Android home screen icon

## Implementation Steps

1. **Create/Obtain Logo Designs**
   - Design dark and light versions of the logo
   - Ensure both versions are visible on their respective backgrounds
   - Optimize SVG files for web (remove unnecessary elements, optimize paths)

2. **Create Favicon**
   - Create a simplified version suitable for small sizes
   - Test visibility at 16x16 pixels
   - Ensure it's recognizable even when tiny

3. **Optimize Files**
   - Compress SVG files (use tools like SVGO)
   - Ensure file sizes are within limits
   - Test in different browsers

4. **Place Files**
   - Place `dark.svg` and `light.svg` in `/logo/` directory
   - Place `favicon.svg` in the root `/` directory

5. **Test**
   - Test logos in both light and dark themes
   - Verify favicon displays correctly in browser tabs
   - Check on different devices and browsers

## Tools and Resources

### SVG Optimization

- **SVGO**: Command-line tool for optimizing SVG files
- **Online tools**: Various online SVG optimizers available

### Design Tools

- **Adobe Illustrator**: Professional vector design
- **Figma**: Web-based design tool
- **Inkscape**: Free, open-source vector editor

### Testing

- Test logos in the Mintlify preview (`mintlify dev`)
- Check favicon in multiple browsers (Chrome, Firefox, Safari, Edge)
- Test on different screen sizes and resolutions

## Current Configuration

The `mint.json` file is already configured to use:

```json
{
  "logo": {
    "dark": "/logo/dark.svg",
    "light": "/logo/light.svg"
  },
  "favicon": "/favicon.svg"
}
```

Once you create and place the files in the correct locations, they will automatically be used by the documentation site.

## Notes

- Logo files should be created by a designer familiar with the Call24x7 brand
- The design should reflect the AI-powered phone calls concept
- Consider accessibility - ensure sufficient contrast for readability
- Test thoroughly before deploying to production

## Support

If you need help with logo/favicon setup:

- Check Mintlify documentation for logo requirements
- Contact support: support@call24x7.ai

