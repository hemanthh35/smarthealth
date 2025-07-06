# HealthAI - Comprehensive Health Management Platform

A modern, AI-powered health management platform that provides comprehensive health monitoring, medical imaging analysis, hospital finder, and symptom assessment capabilities.

## 🚀 Features

### 🏥 **Health Dashboard**
- **Real-time Health Metrics**: Track vital signs, symptoms, and health trends
- **Recent Analyses**: View history of medical imaging and symptom analyses
- **Health Insights**: AI-powered health recommendations and insights
- **Reminder System**: Medication and appointment reminders
- **Health Trends**: Visual charts showing health progress over time
- **Quick Actions**: Fast access to all health tools

### 🔬 **Medical Imaging Analysis**
- **X-Ray Analysis**: AI-powered bone structure and abnormality detection
- **Bone Fracture Detection**: Specialized fracture identification
- **Brain Tumor Detection**: Brain scan analysis for mass detection
- **Ollama LLaVA Integration**: Real AI analysis using local LLaVA model
- **Professional Medical Focus**: Serious medical imaging analysis only

### 🏥 **Hospital & Healthcare Finder**
- **Real-time Location**: Find nearest hospitals, clinics, and pharmacies
- **Multiple Facility Types**: Hospitals, clinics, pharmacies, emergency rooms
- **Interactive Map**: Leaflet-based map with facility markers
- **Distance Calculation**: Accurate distance and travel time estimates
- **Contact Information**: Direct phone numbers and navigation
- **Emergency Alerts**: Quick access to emergency services
- **Filtering Options**: Filter by facility type and services

### 🩺 **Symptom Checker**
- **Comprehensive Symptom Database**: Categorized symptoms (Respiratory, Digestive, Neurological, etc.)
- **Smart Search**: Quick symptom finding with search functionality
- **AI Analysis**: Instant health insights based on symptom patterns
- **Severity Assessment**: Understand symptom severity levels
- **Personalized Recommendations**: Tailored health advice
- **Emergency Warnings**: Alerts for severe symptoms

### 🧠 **AI-Powered Analysis**
- **Ollama LLaVA Model**: Local AI processing for privacy
- **Medical Imaging**: X-ray, bone fracture, and brain tumor analysis
- **Symptom Analysis**: Pattern recognition and condition assessment
- **Confidence Scoring**: AI confidence levels for each analysis
- **Professional Recommendations**: Medical-grade advice and next steps

## 🛠️ Tech Stack

- **Next.js 14** - React framework with App Router
- **TypeScript** - Type-safe development
- **Tailwind CSS** - Modern styling with blue/white theme
- **Lucide React** - Beautiful icons
- **Framer Motion** - Smooth animations
- **Ollama LLaVA** - Local AI model for medical analysis
- **Leaflet** - Interactive maps for hospital finder
- **Overpass API** - Real healthcare facility data
- **Formidable** - File upload handling

## 📦 Installation

### Prerequisites
1. **Node.js** (v18 or higher)
2. **Ollama** - Install from [https://ollama.ai](https://ollama.ai)

### Setup Steps

1. **Clone the repository:**
   ```bash
   git clone <repository-url>
   cd health-ai-platform
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Install Ollama LLaVA model:**
   ```bash
   ollama pull llava
   ```

4. **Start Ollama service:**
   ```bash
   ollama run llava
   ```

5. **Run the development server:**
   ```bash
   npm run dev
   ```

6. **Open your browser:**
   Navigate to [http://localhost:3000](http://localhost:3000)

## 🎯 How to Use

### Dashboard
1. **View Health Overview**: Check your health metrics and recent activities
2. **Add Reminders**: Set medication or appointment reminders
3. **Track Progress**: Monitor health trends and improvements
4. **Quick Access**: Navigate to all health tools from one place

### Medical Imaging Analysis
1. **Upload Image**: Select X-ray or brain scan images
2. **Choose Analysis Type**: X-ray, bone fracture, or brain tumor detection
3. **Analyze with LLaVA**: AI processes the image locally
4. **Review Results**: Get detailed analysis with confidence scores
5. **Follow Recommendations**: Medical advice and next steps

### Hospital Finder
1. **Enable Location**: Allow location access for nearby facilities
2. **Select Facility Type**: Choose hospitals, clinics, or pharmacies
3. **View on Map**: Interactive map with facility locations
4. **Get Details**: Distance, contact info, and navigation
5. **Emergency Access**: Quick access to emergency services

### Symptom Checker
1. **Select Symptoms**: Choose from categorized symptom list
2. **Search Symptoms**: Use search bar for specific symptoms
3. **Analyze**: Get AI-powered health insights
4. **Review Results**: See conditions, probabilities, and recommendations
5. **Follow Advice**: Know when to seek medical care

## 🏥 Medical Imaging Analysis

### Supported Analysis Types
- **X-Ray Analysis**: Bone structure, alignment, and abnormalities
- **Bone Fracture Detection**: Fracture lines, displacement, healing status
- **Brain Tumor Detection**: Mass detection and structural abnormalities

### AI Model Requirements
- **Ollama**: Local AI service for privacy
- **LLaVA Model**: Large Language and Vision Assistant
- **Local Processing**: No data sent to external servers

### Analysis Process
1. **Image Upload**: Convert to base64 for AI processing
2. **Specialized Prompts**: Medical imaging-specific analysis prompts
3. **AI Processing**: LLaVA model analyzes the image
4. **JSON Response**: Structured medical analysis results
5. **User Display**: Formatted results with confidence scores

## 🏥 Healthcare Facility Finder

### Supported Facility Types
- **Hospitals**: Full-service medical facilities
- **Clinics**: Outpatient care centers
- **Pharmacies**: Medication and health supplies
- **Emergency Rooms**: Urgent care facilities

### Features
- **Real-time Data**: Live facility information from OpenStreetMap
- **Distance Calculation**: Accurate travel time and distance
- **Contact Information**: Phone numbers and direct navigation
- **Emergency Alerts**: Quick access to emergency services
- **Interactive Map**: Leaflet-based map with facility markers

## 🩺 Symptom Categories

- **Respiratory**: Cough, runny nose, sore throat, shortness of breath
- **Digestive**: Nausea, vomiting, diarrhea, abdominal pain
- **Neurological**: Headache, dizziness, fatigue, confusion
- **Musculoskeletal**: Joint pain, muscle aches, back pain, swelling
- **General**: Fever, chills, sweating, weight loss

## ⚠️ Important Disclaimers

- This platform is for **informational purposes only**
- **Not a substitute** for professional medical advice
- Always consult with healthcare providers for proper diagnosis
- Seek immediate medical attention for severe symptoms
- AI analysis should be validated by medical professionals

## 🚨 Emergency Notice

If you experience:
- Chest pain
- Difficulty breathing
- Severe symptoms
- Medical emergency

**Call 911 immediately**

## 🎨 User Interface

### Design Theme
- **Blue & White**: Consistent medical theme
- **Modern UI**: Clean, professional interface
- **Responsive Design**: Works on all devices
- **Accessibility**: WCAG compliant design

### Navigation
- **Global Navigation Bar**: Easy access to all features
- **Mobile Responsive**: Touch-friendly interface
- **Quick Actions**: Fast access to common tasks
- **User Menu**: Account and settings access

## 🔧 Development

### Project Structure
```
├── app/                    # Next.js app directory
│   ├── dashboard/         # Health dashboard
│   ├── hospitals/         # Hospital finder
│   ├── app/              # Symptom checker & image analysis
│   ├── api/              # API routes
│   └── globals.css       # Global styles
├── components/            # React components
│   ├── NavigationBar.tsx # Global navigation
│   ├── ImageAnalyzer.tsx # Medical imaging analysis
│   ├── HospitalFinder.tsx # Healthcare facility finder
│   ├── SymptomChecker.tsx # Symptom analysis
│   └── Dashboard.tsx     # Health dashboard
├── lib/                  # Utility libraries
│   └── healthData.ts     # Health data management
├── types/                # TypeScript types
│   └── health.ts         # Health data types
└── pages/api/            # API endpoints
    └── analyze-image.js  # Image analysis API
```

### Available Scripts
- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run start` - Start production server
- `npm run lint` - Run ESLint

### Environment Setup
```bash
# Required for medical imaging analysis
ollama pull llava
ollama run llava

# Development server
npm run dev
```

## 🚀 Deployment

### Production Build
```bash
npm run build
npm run start
```

### Ollama Requirements
- **Local Installation**: Ollama must be installed on the server
- **LLaVA Model**: Must be pulled and running
- **Port 11434**: Default Ollama API port
- **Memory Requirements**: LLaVA model requires significant RAM

## 📱 Mobile Experience

The application is fully responsive and optimized for:
- **Smartphones**: Touch-friendly interface
- **Tablets**: Optimized layouts
- **Desktop**: Full feature access
- **All Browsers**: Cross-browser compatibility

## 🔒 Privacy & Security

- **Local AI Processing**: No medical data sent to external servers
- **Ollama Integration**: All AI analysis done locally
- **No Data Storage**: Images processed but not stored
- **Medical Disclaimer**: Clear warnings about AI limitations

## 🤝 Contributing

This is a comprehensive health management platform showcasing:
- Modern web development practices
- AI integration for healthcare
- Real-time data processing
- Medical-grade user experience

## 📄 License

This project is for educational and demonstration purposes.

---

**Medical Disclaimer**: This platform provides general health information and should not replace professional medical advice. Always consult with healthcare providers for proper diagnosis and treatment. AI analysis results should be validated by qualified medical professionals. 
