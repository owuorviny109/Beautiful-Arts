# Beautiful Arts Gallery

A modern, responsive website for the Beautiful Arts Gallery - Museum of Arts showcasing a blend of modern and medieval ages.

## Live Deployments

**GitHub Pages:** [https://owuorviny109.github.io/Beautiful-Arts/](https://owuorviny109.github.io/Beautiful-Arts/)

**AWS S3 Static Hosting:** [http://beautiful-arts-gallery.s3-website-us-east-1.amazonaws.com](http://beautiful-arts-gallery.s3-website-us-east-1.amazonaws.com)

## Pages Completed

### 1. Home Page (index.html)
- Hero section with background image
- Fully functional navigation bar
- Gallery preview section
- Footer with copyright information

### 2. Contact Us (contact.html)
- Contact form integrated with Formspree
- Contact information display
- Social media links
- Consistent navigation and styling

### 3. About Us (about.html)
- Gallery story and mission
- What we offer section
- Core values display
- Call-to-action buttons

### 4. Sponsorship (sponsorship.html)
- Three sponsorship tiers (Bronze, Silver, Gold)
- Corporate partnership information
- Alternative support options
- Detailed benefits for each tier

## Navigation Structure

All pages include:
- Responsive navbar with logo
- Home link
- Gallery link (scrolls to gallery section on home page)
- Dropdown menu with:
  - Sponsorship
  - About Us
  - Contact Us
- Search functionality
- Mobile-friendly hamburger menu

## Technologies Used

- HTML5
- Bootstrap 5.3.8
- SASS/SCSS for custom styling
- Google Fonts (Poppins)
- Formspree for contact form

## Hosting & Deployment

### GitHub Pages
- Automatic deployment from main branch
- Custom domain support
- HTTPS enabled by default
- Free hosting for public repositories

### AWS S3 Static Website Hosting - Complete Implementation

#### Core S3 Configuration
- **S3 Bucket**: `beautiful-arts-gallery`
- **Static Website Hosting**: Enabled with `index.html` as index document
- **Public Access Policy**: Configured for read-only public access
- **Bucket Policy**: JSON policy allowing `s3:GetObject` for all visitors
- **Regional Deployment**: Optimized for performance and cost

#### Advanced S3 Features Implemented

##### Analytics & Monitoring
- **Server Access Logging**: Enabled with `access-logs/` prefix
  - Tracks visitor IP addresses, timestamps, and requested resources
  - Provides detailed analytics for traffic patterns
  - Logs stored in same bucket for cost efficiency

- **Request Metrics**: Configured for comprehensive monitoring
  - Real-time request count tracking
  - Data transfer monitoring
  - Error rate analysis
  - Performance metrics dashboard

##### Cost Optimization
- **Lifecycle Policies**: Automated storage management
  - Rule name: `optimize-storage`
  - Automatic transition to Standard-IA after 30 days
  - Reduces storage costs for older files
  - Maintains accessibility while optimizing expenses

- **Storage Class Optimization**: 
  - Current files in S3 Standard for optimal performance
  - Automated migration to cheaper storage classes
  - Intelligent cost management without manual intervention

##### Security & Access Control
- **Principle of Least Privilege**: Read-only public access
- **Bucket-Level Security**: Isolated permissions per bucket
- **No Write Access**: Prevents unauthorized modifications
- **AWS Account Isolation**: Website access doesn't expose AWS credentials

## Color Scheme

- Primary: #4F3130 (Dark Brown)
- Secondary: #AA5042 (Terracotta)
- Warning/Accent: #D8BD8A (Gold)



## Features

### Website Features
- Fully responsive design
- Consistent navigation across all pages
- Working contact form
- Professional layout and styling
- Accessible and semantic HTML
- Cross-browser compatible

### Deployment Features
- **Multi-platform deployment** (GitHub Pages + AWS S3)
- **Enterprise-grade hosting** with AWS infrastructure
- **Automated analytics** and visitor tracking
- **Cost optimization** through intelligent storage management
- **Performance monitoring** with real-time metrics
- **Scalable architecture** ready for high traffic
- **Professional DevOps practices** with infrastructure as code principles

### Learning Outcomes Demonstrated
- **Static Website Hosting**: Multiple platform deployment strategies
- **AWS Cloud Services**: Hands-on experience with S3, lifecycle policies, and monitoring
- **Cost Management**: Implementation of automated cost optimization
- **Security Best Practices**: Proper access control and permission management
- **Analytics Implementation**: Server-side logging and metrics collection
- **Infrastructure Documentation**: Comprehensive technical documentation

## Deployment Architecture

This project demonstrates modern web deployment strategies with enterprise-grade features:

### Multi-Platform Strategy
- **GitHub Pages**: Version-controlled deployment with automatic updates
- **AWS S3**: Cloud-native static hosting with enterprise-grade infrastructure
- **Dual Hosting**: Redundancy and platform comparison for learning purposes

### AWS Infrastructure Benefits
- **Scalability**: Handles traffic spikes automatically
- **Reliability**: 99.999999999% (11 9's) durability
- **Global Reach**: AWS global infrastructure
- **Cost Efficiency**: Pay-per-use model with free tier benefits

### Monitoring & Analytics Capabilities
- **Real-time Metrics**: Request counts, data transfer, error rates
- **Access Logs**: Detailed visitor behavior analysis
- **Performance Tracking**: Response times and availability monitoring
- **Cost Monitoring**: Automated expense tracking and optimization

## Technical Implementation Details

### File Structure in S3
```
beautiful-arts-gallery/
├── index.html                 # Main landing page
├── about.html                 # About page
├── contact.html               # Contact form page
├── sponsorship.html           # Sponsorship information
├── gallery.html               # Gallery showcase
├── donate.html                # Donation page
├── assets/                    # Static assets
│   ├── images/               # Art gallery images
│   ├── style/css/            # Compiled CSS files
│   └── svg/                  # SVG icons and graphics
└── access-logs/              # Server access logs (auto-generated)
    ├── 2024-11-11-log1       # Daily visitor logs
    └── ...                   # Historical access data
```

### AWS Services Utilized
- **Amazon S3**: Static website hosting and storage
- **S3 Lifecycle Management**: Automated cost optimization
- **CloudWatch**: Basic monitoring and metrics (via S3 integration)
- **AWS Certificate Manager**: Ready for SSL/TLS if CloudFront is added

### Cost Analysis
- **Current Setup**: ~$0.01-$0.50/month (within free tier limits)
- **After Free Tier**: ~$1-3/month for typical traffic
- **Optimization Features**: Automatic cost reduction through lifecycle policies
- **Monitoring**: Free basic metrics, detailed analytics available

