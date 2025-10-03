# Chocolate Vending Machine System

**GitHub Repository:** https://github.com/TomasTouma/Chocolates_Vending_Machine

A Java Swing-based vending machine simulation that allows customers to purchase chocolate bars and provides administrative controls for inventory management.

![Java](https://img.shields.io/badge/Java-Swing-blue)
![Version](https://img.shields.io/badge/Version-1.0-green)

## 📁 Repository

- **GitHub URL:** https://github.com/TomasTouma/Chocolates_Vending_Machine
- **Clone Command:** `git clone https://github.com/TomasTouma/Chocolates_Vending_Machine`
- **Main Branch:** `main`
- **Project Structure:** Standard NetBeans Java Project

## 📋 Features

### Customer Features
- **Coin Insertion**: Support for 10c, 20c, 50c, €1, and €2 coins
- **Product Selection**: Four chocolate varieties (Twix, KitKat, Mars, Kinder)
- **Automatic Change Calculation**: Intelligent coin-based change dispensing
- **Real-time Inventory Display**: Live stock level updates
- **Money Withdrawal**: Cancel transaction and retrieve inserted coins

### Administrative Features
- **Secure Login**: Password-protected admin access
- **Inventory Management**: Add/remove chocolate bars and coins
- **Real-time Monitoring**: View current stock levels and machine money
- **Dual Interface Updates**: Changes reflect immediately in both admin and customer views

## 🏗️ System Architecture

### Core Components
- **mainScreen.java**: Main customer interface for vending operations
- **LoginFrame.java**: Secure authentication for administrative access
- **addStockFrame.java**: Inventory management interface

### Supported Products & Prices
| Product | Price | Initial Stock |
|---------|-------|---------------|
| Twix    | €1.40 | 10 units      |
| KitKat  | €2.20 | 10 units      |
| Mars    | €1.40 | 10 units      |
| Kinder  | €1.60 | 10 units      |

### Coin System
| Denomination | Initial Quantity |
|--------------|------------------|
| 10-cent      | 20 coins         |
| 20-cent      | 15 coins         |
| 50-cent      | 10 coins         |
| 1-euro       | 10 coins         |
| 2-euro       | 10 coins         |

## 🚀 Quick Start

### Prerequisites
- Java JDK 8 or higher
- NetBeans IDE (recommended)

### Installation & Running
1. **Clone or download** the project files
2. **Open in NetBeans**: File → Open Project → Select project folder
3. **Ensure images are in package**: All PNG images should be in the same package as Java classes
4. **Run the application**: Right-click project → Run File → `mainScreen.java`

### Default Admin Credentials
- **Username**: admin
- **Password**: admin

### GitHub Installation (Recommended)
```bash
git clone https://github.com/TomasTouma/Chocolate-Vending-Machine.git
cd Chocolate-Vending-Machine
# Then open in NetBeans as described below

## 🎯 Usage Guide

### For Customers
1. **Insert Coins**: Click coin buttons to add money
2. **Select Product**: Click desired chocolate bar button
3. **Receive Change**: Automatic calculation and dispensing
4. **Collect Product**: Confirmation dialog with product image
5. **Cancel Transaction**: Use "Withdraw" button to retrieve coins

### For Administrators
1. **Access Admin Panel**: Click "Add Stock" button on main screen
2. **Login**: Enter admin credentials (admin/admin)
3. **Manage Inventory**: Use +/- buttons to adjust stock levels
4. **Manage Coins**: Adjust coin quantities as needed
5. **Close**: Return to main customer interface

## 🔧 Technical Details

### Key Classes & Responsibilities

#### mainScreen.java
- Main customer interface and vending logic
- Coin insertion handling and validation
- Purchase processing with change calculation
- Real-time inventory updates

#### LoginFrame.java
- User authentication system
- Secure access control to admin features
- Input validation and error handling

#### addStockFrame.java
- Inventory management interface
- Stock level adjustments for products and coins
- Synchronized updates with main screen

### Important Methods

#### Purchase Processing (`mainScreen.java`)
- `jButtonTwixActionPerformed()`: Handles Twix purchases
- `jButtonKitKatActionPerformed()`: Handles KitKat purchases
- `jButtonWithdrawActionPerformed()`: Coin return functionality

#### Inventory Management (`addStockFrame.java`)
- `jButton[Product]PlsActionPerformed()`: Increase product stock
- `jButton[Product]MinActionPerformed()`: Decrease product stock
- `jButton[Coin]PlsActionPerformed()`: Increase coin quantities

### Image Resources
The project uses the following images (must be in same package):
- `coinsChange.png` - Change dispensing confirmation
- `twix2.png` - Twix product image
- `kitkat2.png` - KitKat product image
- `mars2.png` - Mars product image
- `kinder2.png` - Kinder product image

## ⚙️ Configuration

### Customization Options
- **Product Prices**: Modify price checks in purchase methods
- **Initial Stock**: Adjust static field initial values
- **Admin Credentials**: Change in `LoginFrame.java` authentication logic
- **Coin Denominations**: Modify coin values in calculation methods

### Security Notes
- Current implementation uses hardcoded credentials
- For production use, consider implementing encrypted credential storage
- Admin interface should have additional access controls

## 🐛 Troubleshooting

### Common Issues

**Images not displaying:**
- Ensure image files are in the same package as Java classes
- Check image file names match the code references
- Verify image paths use forward slashes in package structure

**Purchase not completing:**
- Verify sufficient coins are available for change
- Check product stock levels
- Ensure inserted money meets or exceeds product price

**Admin login failing:**
- Verify username: "admin" (case insensitive)
- Verify password: "admin" (case sensitive)
- Check for extra spaces in input fields

### Error Messages
- "Invalid Username or Password" - Admin authentication failed
- "No coins to withdraw" - Withdrawal attempted with no inserted money
- "Purchase can't be completed" - Insufficient funds or out of stock

## 🔄 Maintenance

### Regular Tasks
- Monitor coin levels to ensure change availability
- Restock popular products regularly
- Check machine money total for collection
- Verify all coin mechanisms are functioning

### Best Practices
- Maintain minimum coin levels for change calculation
- Regular backup of any persistent data (if implemented)
- Keep product prices updated in the code
- Test all coin denominations regularly

## 👨‍💻 Development

### Code Structure
- MVC-like architecture with separation of concerns
- Static fields for shared state management
- Event-driven design for user interactions
- Modular methods for maintainability

### Extension Ideas
- Database integration for persistent storage
- Transaction logging and reporting
- Multiple user roles and permissions
- Network connectivity for remote monitoring
- Currency conversion support

### Building from Source
1. **Clone the repository**
   ```bash
   git clone https://github.com/YourUsername/Chocolate-Vending-Machine.git

## 📞 Support

**Author**: Tomasz Touma  
**Version**: 1.0  
**Last Updated**: December 2024

For technical support or questions:
1. Check this README for common solutions
2. Verify all image files are properly located
3. Ensure Java version compatibility
4. Test with default credentials and settings

## 📄 License

This project is available for educational and demonstration purposes. Please ensure proper attribution for any reuse or modification.

---

*Enjoy your chocolate vending experience! 🍫*