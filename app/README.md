# FitRater

FitRater is a fashion-focused iOS application that allows users to upload their outfits and receive a generated rating with feedback.

Users can customize their submission by selecting details such as the occasion, outfit type, weather, accessories, and other style preferences before submitting their fit. The app also allows users to track and review previously submitted outfits.

## Requirements

- Xcode 15 or newer
- Swift 5
- iOS 16+ recommended
- Internet connection required for authentication
- Firebase Authentication configured for email/password login and registration
- No additional pods required beyond Firebase setup

## Testing Instructions

- Recommended simulator: iPhone 14 or newer
- Orientation: Portrait mode only
- The application may also be tested on a real iPhone
- A real iPhone is recommended for testing haptic feedback

### Test Account

- Email: `ridisha.saquib@gmail.com`
- Password: **Available upon request**

> Note: Do not store real account passwords in a public GitHub repository.

## Main Features

### Settings

- Light/Dark mode toggle
- Haptics on/off
- Fit rating strictness:
  - Easy
  - Normal

### Custom UI

- `SnellRoundhand-Bold` font
- Custom soft blue buttons
- Pink accent elements
- Rounded UI components
- Styled layouts

### Major Components

- Firebase email/password login and registration
- User profile with camera and photo library integration

### Additional UI Elements

- Segmented controls
  - Occasion selection
  - Rating strictness
- Switches
  - Accessories
  - Colors
  - Haptics

## Navigation and Structure

- Tab Bar Controller
- Table View for outfit history
- Scroll/Stack View for the Rate tab

## iOS Features Used

- Alerts
  - Error messages
  - Delete confirmations
  - Missing information
- Action Sheets
  - Photo upload options
- Stack Views
- Scroll Views
- Haptic feedback
- UserDefaults

## Frameworks and Advanced Features

- Firebase Authentication
- Animation
  - Fit Scan screen includes a bouncing bow animation

## Haptics

Haptic feedback is used throughout the application, including:

- Rate tab
- History tab
- Profile tab

> Haptics only work when running the application on a physical iPhone.

## Changes From Original Project Proposal

Overall, FitRater follows the original Project Part 1 plan, with several design and implementation changes made to improve usability and visual appeal.

### Button Design

The original button designs were changed to create a more visually appealing interface.

### Rate Tab Validation

Instead of displaying an alert when required outfit information is missing, the **Rate My Fit** button remains disabled until the user completes all required fields.

### Rating Strictness

The original proposal included a strictness slider ranging from 1–20. This was replaced with a segmented control containing two options:

- Easy
- Normal

This change was made because the segmented control provides a simpler and more understandable way for users to select their desired rating strictness.

The results screen also displays the rating mode selected by the user.
