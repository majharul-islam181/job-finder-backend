## job-notifier-backend
```
job-notifier-backend/
├── src/
│   ├── config/
│   │   ├── db.js               # MongoDB connection setup
│   │   ├── firebase.js         # Firebase Admin SDK initialization
│   │   └── scraperSites.js     # List of websites to scrape
│   │
│   ├── controllers/
│   │   ├── jobController.js    # Handles job fetching and response
│   │   ├── userController.js   # (optional) Handles user subscriptions
│   │
│   ├── models/
│   │   ├── Job.js              # Job schema (title, company, url, etc.)
│   │   ├── User.js             # (optional) User schema if needed
│   │
│   ├── routes/
│   │   ├── jobRoutes.js        # `/api/jobs` endpoints
│   │   ├── userRoutes.js       # `/api/users` endpoints
│   │
│   ├── services/
│   │   ├── notificationService.js  # Send push notification logic
│   │   ├── scraperService.js       # Scraping logic for career pages
│   │
│   ├── scraper/
│   │   ├── companies/
│   │   │   ├── googleScraper.js    # Scraper for Google's career page
│   │   │   ├── amazonScraper.js    # Scraper for Amazon's career page
│   │   │   └── (others...)         # Add more companies easily
│   │   └── scraperManager.js       # Manages multiple scrapers
│   │
│   ├── middlewares/
│   │   ├── errorMiddleware.js      # Global error handler
│   │   └── asyncHandler.js          # Catch async errors
│   │
│   ├── jobs/
│   │   └── jobScheduler.js          # Cron job that runs every 5 mins
│   │
│   ├── utils/
│   │   ├── logger.js                # For logging (info, errors)
│   │   └── helperFunctions.js       # Any small reusable functions
│   │
│   ├── app.js                       # Express app setup
│   └── server.js                    # Server startup file
│
├── Dockerfile                        # Docker setup (optional)
├── docker-compose.yml                # For app + MongoDB together (optional)
├── .env                               # Environment variables
├── package.json
├── README.md


```
