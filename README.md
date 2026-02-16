# Campus Monitor Dashboard

A real-time crowdsourced campus monitoring system for students to track availability and occupancy across various campus locations.

## Features

- 🍽️ **Mess Status**: Food availability tracking
- 🏫 **Classrooms (LH1-LH9)**: Occupancy status for 9 lecture halls
- 🏋️ **Gym**: Real-time headcount and crowd levels
- 📚 **Library**: Separate tracking for Ground Floor and First Floor occupancy
- ☕ **Student Centre**: Nescafe and Nandini open/closed status
- 🏸 **Badminton Courts**: Individual court occupancy (4 courts)
- 👨‍🏫 **Faculty Availability**: Real-time availability status for 12 faculty members

## How It Works

### Crowdsourced Updates
- Students can update status for any location
- **Confirmation System**: Most locations require 3 student confirmations to change status
- **Student Centre**: Requires only 2 confirmations (faster updates)
- **Badminton Courts**: Requires only 2 confirmations
- **Auto-Expiry**: Status automatically expires after 30 minutes if not updated

### Number-Based Reporting
For more objective tracking:
- **Gym**: Students report actual headcount (averaged from last 3 reports)
- **Library Floors**: Students report actual headcount (averaged from last 3 reports)
- **Badminton Courts**: Students report number of occupied courts (averaged from last 3 reports)

### Faculty Updates
- Password protected: `baseufac`
- Only authorized users can update faculty availability
- 4 status options: Available, In Class, In Meeting, Out of Office

## Deployment Instructions

### Option 1: GitHub Pages (Recommended)

1. **Create a GitHub Repository**
   - Go to [github.com](https://github.com) and sign in
   - Click the "+" icon in the top right → "New repository"
   - Repository name: `campus-monitor` (or any name you prefer)
   - Make it **Public**
   - Click "Create repository"

2. **Upload the File**
   - Click "uploading an existing file"
   - Drag and drop `index.html` or click "choose your files"
   - Commit changes (add a message like "Initial commit")

3. **Enable GitHub Pages**
   - Go to your repository **Settings**
   - Scroll down to **Pages** section (in the left sidebar)
   - Under "Source", select **main** branch
   - Click **Save**

4. **Access Your Site**
   - Your dashboard will be live at: `https://yourusername.github.io/campus-monitor`
   - Takes 1-2 minutes to become active
   - Share this link with your campus!

### Option 2: Netlify (Alternative)

1. Go to [netlify.com](https://netlify.com)
2. Sign up/login (free account)
3. Drag and drop the `index.html` file onto the Netlify dashboard
4. Get instant URL like: `your-campus-monitor.netlify.app`

### Option 3: University Web Hosting

If your university provides web hosting:
1. Contact your IT department for FTP/SFTP credentials
2. Upload `index.html` to your web space
3. Access via your university's URL structure

## Usage Guide

### For Students

**Viewing Status:**
- Simply open the dashboard URL on any device
- Click any location card to see detailed status
- No login required to view

**Updating Status:**
- Click on any location card
- Select/enter the current status
- Your vote will be recorded
- Status changes after required confirmations are met

**Tips:**
- Bookmark the dashboard for quick access
- Update status when you visit a location
- More accurate updates = better experience for everyone

### For Faculty

**Updating Your Availability:**
1. Click on "Faculty" card
2. Click your name
3. Enter password: `baseufac`
4. Select your current status (Available/In Class/In Meeting/Out of Office)
5. Status updates immediately

### For Mess Staff (Optional Manual Updates)

While the system is designed for student updates, staff can also update:
1. Click "Mess" card
2. Select "Food Available" or "Food Finished"
3. After 3 confirmations (can be same person voting 3 times), status updates

## Technical Details

- **Technology**: Pure HTML, CSS, JavaScript (no external dependencies)
- **Storage**: Browser localStorage (data persists locally)
- **Responsive**: Works on mobile, tablet, and desktop
- **Offline Capable**: Works without internet after first load
- **No Backend Required**: Completely client-side application

## Data Privacy

- No personal data is collected
- All data stored locally in browser
- No tracking or analytics
- No server-side storage

## Customization

You can easily customize:
- **Confirmation thresholds**: Edit values in the JavaScript code
- **Auto-expiry time**: Change `AUTO_EXPIRY_TIME` constant
- **Location names**: Modify room numbers, faculty names, etc.
- **Colors and styling**: Edit CSS section
- **Add more locations**: Extend the data structure

## Troubleshooting

**Status not updating?**
- Make sure enough confirmations are received
- Check if status has expired (30+ minutes old)
- Clear browser cache and reload

**Faculty password not working?**
- Password is case-sensitive: `baseufac`
- Make sure there are no extra spaces

**Dashboard not loading?**
- Check internet connection (first load only)
- Try a different browser
- Clear browser cache

## Future Enhancements

Potential additions:
- Analytics dashboard for admin
- Push notifications for status changes
- Historical data tracking
- Mobile app version
- Integration with university systems

## Support

For issues or feature requests, contact your campus IT team or the project maintainer.

## License

Free to use and modify for educational purposes.

---

**Made with ❤️ for campus convenience**