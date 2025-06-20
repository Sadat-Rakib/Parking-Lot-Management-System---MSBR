# Parking-Lot-Management-System---MSBR

# 🚗 Parking Lot Management System

A comprehensive web-based parking lot management solution built with vanilla HTML, CSS, and JavaScript. Features real-time visual parking spot management, vehicle tracking, and intuitive drag-and-drop functionality.

## ✨ Features

- **Interactive Visual Interface** - Real-time parking lot visualization with color-coded spots
- **Multi-Floor Support** - Manage multiple parking floors simultaneously  
- **Vehicle Types** - Support for Cars, Bikes, and Trucks with dedicated spots
- **Drag & Drop** - Move vehicles between spots with intuitive drag-and-drop
- **Search Functionality** - Quickly locate vehicles by license plate
- **Spot Analytics** - Count available spots by type and floor
- **Responsive Design** - Works seamlessly on desktop and mobile devices
- **Toast Notifications** - Real-time feedback for all parking operations

## 🚀 Demo

Simply open `index.html` in your web browser to start using the application immediately - no installation required!

## 📋 How to Use

### Parking a Vehicle
1. Click on any available (green) parking spot
2. Enter the vehicle number in the modal dialog
3. Click "Submit" to park the vehicle

### Moving a Vehicle
- Drag any occupied spot to an available spot to relocate the vehicle

### Unparking a Vehicle
- Click on any occupied (red) spot and confirm to unpark

### Search for a Vehicle
1. Enter vehicle number in the search box
2. Click "Search" to find the exact location

### Check Available Spots
1. Select vehicle type and floor from the dropdown
2. Click "Count" to see available spots

## 🏗️ System Architecture

### Core Classes

#### `ParkingSpot`
- Manages individual parking spot state
- Handles vehicle parking/unparking operations
- Stores vehicle type and occupancy status

#### `ParkingFloor` 
- Manages a grid of parking spots (4x5 default)
- Provides floor-level operations and analytics
- Handles vehicle search within the floor

#### `ParkingLot`
- Orchestrates multiple parking floors
- Provides system-wide vehicle management
- Coordinates all parking operations

## 🎨 Visual Design

- **Available Spots**: Green background with vehicle type indicator
- **Occupied Spots**: Red background with vehicle number display
- **Responsive Grid**: Adapts to different screen sizes
- **Modern UI**: Clean, professional interface with smooth animations

## 📱 Browser Compatibility

- ✅ Chrome 60+
- ✅ Firefox 55+
- ✅ Safari 12+
- ✅ Edge 79+

## 🔧 Configuration

Default configuration creates:
- 2 parking floors
- 4 rows × 5 columns per floor (20 spots per floor)
- Alternating spot types: Car, Bike, Truck

To modify the parking lot size, update the initialization:
```javascript
const parkingLot = new ParkingLot(floors, rows, columns);
```

## 📝 Technical Features

- **No Dependencies** - Pure vanilla JavaScript implementation
- **Local State Management** - All data stored in browser memory
- **Event-Driven Architecture** - Responsive user interactions
- **CSS Grid Layout** - Modern, flexible positioning
- **ES6+ Features** - Modern JavaScript syntax and features

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🆘 Support

If you encounter any issues or have questions:
- Open an issue on GitHub
- Check the code comments for implementation details
- Review the browser console for any error messages

## 🎯 Future Enhancements

- [ ] Persistent data storage
- [ ] Payment integration
- [ ] Time-based parking
- [ ] Advanced reporting
- [ ] Admin dashboard
- [ ] API integration

---

**Made with ❤️ for efficient parking management**
