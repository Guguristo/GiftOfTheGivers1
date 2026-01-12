# GiftOfGivers - Charitable Donation Platform

GiftOfGivers is a comprehensive web-based platform designed to streamline charitable donations and community support initiatives. The application enables registered users to contribute various resources—such as food, clothing, cash, or services—directly to verified charitable projects or organizations.

## 🚀 Features

### Core Functionality
- **User Authentication & Registration**: Secure user accounts with profile management
- **Donation Management**: Track and manage charitable donations of all types
- **Organization Integration**: Connect with verified charitable organizations
- **Impact Tracking**: Monitor your giving history and community impact
- **Dashboard Analytics**: Visual statistics of your charitable contributions

### Donation Types Supported
- 🍎 **Food**: Canned goods, fresh produce, non-perishables
- 👕 **Clothing**: Gently used or new clothing items
- 💰 **Cash**: Monetary donations with estimated value tracking
- 🛠️ **Services**: Volunteer time and professional services
- 📦 **Other**: Any other charitable contributions

### User Experience Features
- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **Modern UI**: Clean, intuitive interface with Bootstrap 5 and Font Awesome icons
- **Real-time Statistics**: Live updates of donation counts and values
- **Secure Transactions**: Industry-standard security for user data protection

## 🛠️ Technology Stack

- **Framework**: ASP.NET Core 8.0 (MVC)
- **Database**: SQL Server with Entity Framework Core
- **Authentication**: ASP.NET Core Identity
- **Frontend**: Bootstrap 5, Font Awesome, jQuery
- **Styling**: Custom CSS with modern design principles

## 📋 Prerequisites

Before running this application, ensure you have:

- [.NET 8.0 SDK](https://dotnet.microsoft.com/download/dotnet/8.0)
- [SQL Server LocalDB](https://docs.microsoft.com/en-us/sql/database-engine/configure-windows/sql-server-express-localdb) or SQL Server
- [Visual Studio 2022](https://visualstudio.microsoft.com/downloads/) or [Visual Studio Code](https://code.visualstudio.com/)

## 🚀 Getting Started

### 1. Clone the Repository
```bash
git clone <repository-url>
cd Guguweb
```

### 2. Restore Dependencies
```bash
dotnet restore
```

### 3. Update Database Connection
Edit `appsettings.json` to match your database configuration:
```json
{
  "ConnectionStrings": {
    "DefaultConnection": "Server=(localdb)\\mssqllocaldb;Database=GiftOfGiversDb;Trusted_Connection=true;MultipleActiveResultSets=true"
  }
}
```

### 4. Build and Run
```bash
dotnet build
dotnet run
```

### 5. Access the Application
Open your browser and navigate to `https://localhost:7000` (or the port shown in the console)

## 📊 Database Schema

### Core Entities

#### ApplicationUser
- Extended Identity user with additional profile information
- FirstName, LastName, Address, City, State, ZipCode
- DateJoined, IsActive status
- Navigation to Donations

#### Organization
- Verified charitable organizations
- Contact information and location details
- Verification status and active status
- Navigation to Donations

#### Donation
- Core donation entity with comprehensive tracking
- Type (Food, Clothing, Cash, Services, Other)
- Item description, quantity, estimated value
- Status tracking (Pending, Approved, Delivered, Cancelled)
- Delivery information and instructions
- Links to User and Organization

## 🎯 Key Features Implementation

### Authentication System
- Secure user registration and login
- Password requirements and validation
- User profile management
- Session management with remember me functionality

### Donation Management
- Create, read, update, delete donations
- Comprehensive donation tracking
- Status management workflow
- Delivery scheduling and instructions

### Dashboard Analytics
- Personal giving statistics
- Donation type breakdown
- Monthly donation tracking
- Recent donation history
- Impact visualization

### Organization Integration
- Pre-seeded verified organizations
- Organization selection for donations
- Contact information display
- Partnership tracking

## 🎨 UI/UX Features

### Modern Design
- Clean, professional interface
- Consistent color scheme and typography
- Responsive grid layout
- Interactive elements with hover effects

### User Experience
- Intuitive navigation
- Clear call-to-action buttons
- Form validation with helpful error messages
- Loading states and feedback

### Accessibility
- Semantic HTML structure
- ARIA labels and descriptions
- Keyboard navigation support
- Screen reader compatibility

## 🔒 Security Features

- ASP.NET Core Identity for authentication
- Password hashing and validation
- CSRF protection
- SQL injection prevention
- Input validation and sanitization

## 📱 Responsive Design

The application is fully responsive and optimized for:
- **Desktop**: Full-featured experience with sidebar navigation
- **Tablet**: Touch-optimized interface with collapsible menus
- **Mobile**: Streamlined layout with mobile-first design

## 🚀 Deployment

### Local Development
1. Ensure SQL Server LocalDB is installed
2. Run `dotnet run` from the project directory
3. Access via `https://localhost:7000`

### Production Deployment
1. Configure production database connection string
2. Set up SSL certificates
3. Configure logging and monitoring
4. Deploy to Azure, AWS, or on-premises server

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Bootstrap team for the excellent CSS framework
- Font Awesome for the comprehensive icon library
- Microsoft for ASP.NET Core and Entity Framework
- The open-source community for inspiration and tools

## 📞 Support

For support, email support@giftofgivers.org or join our community forum.

---

**GiftOfGivers** - Making a difference in our community through charitable giving. 💝
