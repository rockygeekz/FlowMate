# FlowMate

A comprehensive workflow automation platform that streamlines business processes through intelligent automation and data extraction capabilities. Built with modern web technologies to provide a scalable, secure, and user-friendly automation solution.

![Dashboard Overview](./flow_mate_dashboard.png)

![Workflow Builder Interface](./flow_mate_editor.png)

![Execution Results Dashboard](./flow_mate_execution.png)

## Core Features

**Workflow Management**
- Visual workflow builder with drag-and-drop functionality
- Multi-step automation with phase-based execution
- Real-time workflow monitoring and status tracking
- Scheduled execution with customizable timing

**Data Extraction & Processing**
- Integrated web scraping capabilities
- Support for complex data extraction workflows  
- Automated data validation and processing
- Export functionality for extracted data

**Security & Credentials**
- Encrypted credential storage system
- Secure API key management
- User authentication with session handling
- Role-based access control

**Analytics & Monitoring**
- Comprehensive dashboard with real-time metrics
- Workflow performance analytics
- Usage tracking and reporting
- Error logging and debugging tools

**AI Integration**
- Intelligent workflow assistant
- AI-powered optimization suggestions
- Automated troubleshooting guidance
- Smart workflow recommendations

## Technology Stack

**Frontend Architecture**
- Next.js 14 with App Router
- TypeScript for type safety
- Tailwind CSS for styling
- ShadCn UI component library
- React Hook Form for form management

**Backend Infrastructure**
- Next.js Server Actions for API handling
- PostgreSQL database with Prisma ORM
- NextAuth.js for authentication
- JWT token management
- Server-side rendering optimization

**External Integrations**
- Stripe for payment processing and subscriptions
- OpenAI API for AI-powered features
- Email service integration
- Third-party API connectors

**Development & Deployment**
- ESLint and Prettier for code quality
- TypeScript strict mode
- Environment-based configuration
- Production-ready build optimization

## Installation & Setup

**Prerequisites**
- Node.js 18+ and npm
- PostgreSQL database
- Stripe account for payments
- OpenAI API key

**Installation Steps**

1. **Clone and Setup**
   ```bash
   git clone https://github.com/Amishmathur1/ScrapifySAAS
   cd ScrapifySAAS
   npm install
   ```

2. **Environment Configuration**
   Create `.env.local` file:
   ```env
   # Database
   DATABASE_URL="postgresql://username:password@localhost:5432/flowmate"
   
   # Authentication
   NEXTAUTH_SECRET="your-secret-key"
   NEXTAUTH_URL="http://localhost:3000"
   
   # AI Integration
   OPENAI_API_KEY="your-openai-api-key"
   
   # Payment Processing
   STRIPE_SECRET_KEY="your-stripe-secret-key"
   STRIPE_PUBLISHABLE_KEY="your-stripe-publishable-key"
   ```

3. **Database Setup**
   ```bash
   npx prisma migrate dev --name init
   npx prisma generate
   ```

4. **Development Server**
   ```bash
   npm run dev
   ```
   Access at `http://localhost:3000`

## Platform Usage

**Getting Started**
- Register account with email verification
- Complete onboarding and profile setup
- Receive initial credits for workflow testing

**Building Workflows**
- Use visual editor to create automation sequences
- Configure data sources and extraction parameters
- Set up conditional logic and error handling
- Test workflows in development environment

**Managing Operations**
- Schedule workflows for automated execution
- Monitor real-time performance metrics
- Review execution logs and error reports
- Manage billing and subscription settings

**AI Assistance**
- Access contextual help through integrated assistant
- Get workflow optimization recommendations
- Troubleshoot issues with intelligent suggestions
- Learn best practices for automation design

## Development Commands

| Command | Description |
|---------|-------------|
| `npm run dev` | Start development server with hot reload |
| `npm run build` | Create optimized production build |
| `npm start` | Run production server |
| `npm run lint` | Run ESLint code analysis |
| `npm run lint:fix` | Auto-fix linting issues |
| `npm run type-check` | Run TypeScript type checking |
| `npm run db:migrate` | Run database migrations |
| `npm run db:studio` | Open Prisma Studio |

## Key Implementations

**Authentication System**
- NextAuth.js with multiple providers
- Secure session management
- Protected routes and middleware
- User role management

**Workflow Engine**
- Custom workflow execution engine
- State management with React Context
- Real-time status updates via WebSocket
- Error handling and recovery mechanisms

**Payment Integration**
- Stripe subscription management
- Usage-based billing system
- Invoice generation and tracking
- Automated payment processing

**Data Management**
- Prisma ORM with PostgreSQL
- Database migrations and seeding
- Optimized queries and indexing
- Data validation and sanitization

## Architecture Highlights

- **Scalable Design**: Modular architecture supporting horizontal scaling
- **Security First**: Comprehensive security measures including data encryption
- **Performance Optimized**: Efficient database queries and caching strategies
- **User Experience**: Responsive design with intuitive navigation
- **Maintainable Code**: TypeScript, proper error handling, and comprehensive testing
