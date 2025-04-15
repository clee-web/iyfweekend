# IYF Academy Deployment Guide

## Prerequisites
- Node.js >= 18.0.0
- npm >= 8.0.0
- SQLite3
- A domain name (for production)
- SSL certificate (for production)

## Deployment Steps

### 1. Environment Setup
- [ ] Set up production environment variables in `.env`
- [ ] Generate a secure JWT_SECRET
- [ ] Configure CORS_ORIGIN with your domain
- [ ] Set up SSL certificate

### 2. Database Setup
- [ ] Ensure database file exists at `./db/iyfacademy.db`
- [ ] Verify database permissions
- [ ] Create backup of existing database

### 3. Server Setup
- [ ] Install dependencies: `npm install`
- [ ] Build frontend: `npm run build`
- [ ] Test server locally: `npm start`

### 4. Production Deployment
- [ ] Set up reverse proxy (e.g., Nginx)
- [ ] Configure SSL/TLS
- [ ] Set up process manager (e.g., PM2)
- [ ] Configure firewall rules
- [ ] Set up monitoring and logging

### 5. Post-Deployment
- [ ] Test all API endpoints
- [ ] Verify admin login
- [ ] Check student registration
- [ ] Monitor server logs
- [ ] Set up automated backups

## Security Checklist
- [ ] Change default admin password
- [ ] Enable HTTPS
- [ ] Configure CORS properly
- [ ] Set up rate limiting
- [ ] Enable security headers
- [ ] Regular security updates

## Maintenance
- Regular database backups
- Monitor server logs
- Update dependencies
- Check SSL certificate expiration
- Regular security audits

## Troubleshooting
1. Check server logs for errors
2. Verify database connection
3. Check environment variables
4. Test API endpoints
5. Monitor server resources

## Contact
For deployment issues, contact the development team. 