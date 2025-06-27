# Bengali Alphabet Learning App

An interactive Android application for learning Bengali alphabet through drawing practice, similar to Duolingo but focused on Bengali characters.

## Features

- **Interactive Drawing**: Practice writing Bengali characters with finger touch gestures
- **Intelligent Feedback**: Get real-time feedback on your drawing accuracy
- **Progressive Guidance**: Adjustable guidance system with dots, arrows, and full path demonstrations
- **Multiple Categories**: Learn vowels, consonants, numbers, and compound letters
- **Progress Tracking**: Track your learning progress across different character categories
- **Audio Support**: Listen to pronunciation and record your own voice for practice

## Technical Details

### Architecture

The app follows the MVVM (Model-View-ViewModel) architecture pattern:

- **Model**: Data classes for Bengali characters, strokes, and user progress
- **View**: Activities and custom views for user interaction
- **ViewModel**: Manages UI state and business logic

### Key Components

1. **DrawingView**: Custom view for interactive character drawing
2. **GestureRecognizer**: Validates user strokes against target patterns
3. **FeedbackManager**: Provides visual and audio feedback during practice
4. **AlphabetRepository**: Manages Bengali alphabet data

### Gesture Recognition System

The app uses a sophisticated gesture recognition system that:

- Samples points along the user's drawn path
- Compares direction, shape, and position to the target stroke
- Calculates accuracy scores for different aspects of the drawing
- Provides specific feedback based on the user's performance

### Guidance System

Four levels of guidance are available:

1. **None**: No guidance, for advanced users
2. **Dots Only**: Shows start and end points for each stroke
3. **Dots and Arrows**: Shows dots with directional arrows
4. **Full Path**: Shows the complete stroke path with animated guidance

## Building and Running

### Prerequisites

- Android Studio 4.0+
- Android SDK 21+
- Kotlin 1.5+

### Setup

1. Clone the repository
2. Open the project in Android Studio
3. Sync Gradle files
4. Build and run on an emulator or physical device

## Project Structure

```
app/
├── src/
│   ├── main/
│   │   ├── java/com/example/bengalialphabetapp/
│   │   │   ├── data/           # Data models
│   │   │   ├── ui/             # Activities and UI components
│   │   │   └── utils/          # Utility classes
│   │   ├── res/                # Resources
│   │   └── assets/alphabets/   # Bengali alphabet data files
│   └── test/                   # Unit tests
└── build.gradle                # App-level build configuration
```

## Future Enhancements

- Add more compound letters and special characters
- Implement handwriting recognition using machine learning
- Add gamification elements like points, badges, and challenges
- Support for other Indic scripts like Hindi, Tamil, etc.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Inspired by language learning apps like Duolingo
- Bengali character data sourced from linguistic resources
- Special thanks to the Bengali language community

