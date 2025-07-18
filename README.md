# finch
# Medical & Finance AI Chatbot

A specialized AI chatbot that provides evidence-based information on healthcare and financial topics with verified sources and expert consultation routing.

## Features

### 🎯 Core Functionality
- **Fine-tuned Knowledge Base**: Curated medical and financial information from reliable sources
- **Smart Categorization**: Automatically detects whether queries are medical, financial, or general
- **Source Citations**: Every response includes credible sources with URLs and credibility indicators
- **Confidence Scoring**: Responses include confidence levels (high/medium/low)

### 🧠 AI Capabilities
- **Empathetic Responses**: Contextually appropriate, caring communication
- **Expert Routing**: Automatic detection when professional consultation is needed
- **Conversation Memory**: Tracks user preferences and consultation history
- **Real-time Processing**: Simulated AI processing with typing indicators

### 🔒 Safety Features
- **Professional Disclaimers**: Clear warnings about seeking professional advice
- **Expert Escalation**: "Connect with Expert" buttons for complex cases
- **Responsible AI**: Prioritizes user safety over comprehensive answers
- **Source Verification**: All information linked to credible institutions

## Knowledge Base Sources

### Medical Sources
- American Heart Association
- Mayo Clinic
- Centers for Disease Control (CDC)
- National Institutes of Health (NIH)
- Food and Drug Administration (FDA)
- WebMD

### Financial Sources
- Securities and Exchange Commission (SEC)
- Consumer Financial Protection Bureau
- Department of Labor
- Financial Planning Association
- Investopedia
- Credit Bureaus (Experian, etc.)

## Installation & Setup

### Option 1: HTML Version (Standalone)
1. Download the HTML file
2. Open in any modern web browser
3. No additional setup required

### Option 2: React Component Version
1. Install dependencies:
   ```bash
   npm install react react-dom lucide-react
   ```
2. Copy the React component code
3. Import and use in your React application

## Usage

### Basic Operation
1. Select a category (General, Medical, Finance)
2. Type your question in the input field
3. Press Enter or click Send
4. Review the response with sources
5. Use "Connect with Expert" for complex cases

### Example Queries

**Medical:**
- "What are the symptoms of a heart attack?"
- "How do I manage my diabetes?"
- "What should I know about blood pressure?"

**Financial:**
- "How should I start investing?"
- "What's the 50/30/20 budget rule?"
- "How do I improve my credit score?"

## Architecture

### Component Structure
```
MedicalFinanceChatbot/
├── State Management (React hooks)
├── Knowledge Base (JSON structure)
├── Message Processing
├── Source Attribution
├── Expert Routing
└── UI Components
```

### Key Functions
- `getResponseCategory()`: Categorizes user input
- `findRelevantInfo()`: Matches queries to knowledge base
- `generateEmpatheticResponse()`: Adds empathetic context
- `requestExpertConsultation()`: Handles expert routing

## Customization

### Adding New Knowledge
```javascript
knowledgeBase.medical["new_topic"] = {
    response: "Your informative response here",
    sources: [
        { title: "Source Name", url: "https://example.com", type: "clinical" }
    ],
    confidence: "high",
    requiresExpert: false
};
```

### Source Types
- `clinical`: Medical journals, clinical guidelines
- `educational`: Educational institutions, health organizations
- `government`: Government health agencies
- `regulatory`: SEC, FDA, other regulatory bodies
- `professional`: Professional associations

### Confidence Levels
- `high`: Well-established, consensus information
- `medium`: Generally accepted but may have nuances
- `low`: Emerging or controversial topics

## Best Practices

### For Medical Content
- Always include appropriate disclaimers
- Prioritize emergency guidance for urgent symptoms
- Include multiple credible sources
- Flag content requiring professional consultation

### For Financial Content
- Include risk warnings for investment advice
- Provide general principles rather than specific recommendations
- Reference regulatory guidelines
- Encourage professional financial planning

### For User Experience
- Keep responses concise but informative
- Use empathetic language for sensitive topics
- Provide clear next steps
- Make expert consultation easily accessible

## Compliance & Legal

### Medical Disclaimer
This chatbot provides general health information for educational purposes only. It is not a substitute for professional medical advice, diagnosis, or treatment. Always seek the advice of qualified healthcare providers.

### Financial Disclaimer
This chatbot provides general financial information for educational purposes only. It is not personalized financial advice. Always consult with qualified financial professionals for investment decisions.

### Data Privacy
- No personal health information is stored
- Conversations are not logged or retained
- All processing happens client-side

## Technical Requirements

### Browser Support
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

### Dependencies
- React 18+
- Lucide React (icons)
- Tailwind CSS (styling)

## Deployment

### Local Development
1. Clone the repository
2. Open `index.html` in your browser
3. Start testing immediately

### Production Deployment
1. Upload HTML file to your web server
2. Ensure HTTPS for security
3. Configure CDN for better performance
4. Set up monitoring and analytics

## Contributing

### Adding Medical Content
1. Verify with multiple credible sources
2. Include appropriate confidence levels
3. Add expert routing for complex topics
4. Test with medical professionals

### Adding Financial Content
1. Reference regulatory guidelines
2. Include risk disclosures
3. Provide educational context
4. Validate with financial experts

## Support

For questions or issues:
1. Check the documentation
2. Review the knowledge base structure
3. Test with sample queries
4. Consult the troubleshooting guide

