# AI-Smart-Fit-Trainer
An AI-powered posture correction, workout coaching, nutrition planning, and exercise analytics platform that combines computer vision, machine learning, and generative AI to help users train with better form and achieve fitness goals safely.
Features
1. Posture Data Trainer

Train a custom logistic regression model directly in the browser.

Import posture datasets via CSV
Manual sample entry
Label posture as Good (1) or Bad (0)
Train using Gradient Descent
Accuracy, Precision, Recall metrics
Confusion Matrix visualization
Model persistence via localStorage
2. Live Posture Classifier

Real-time form evaluation using trained posture models.

Supported Exercises:

Squat
Deadlift
Push-Up
Plank
Overhead Press

Features:

Interactive angle sliders
Confidence scoring
Real-time classification
Session rep logging
3. AI Coach (Anthropic Integration)

Receive personalized coaching after every repetition.

The AI analyzes:

Exercise type
Form classification
Confidence score
Angle deviations
Historical performance

Returns:

Targeted correction
Positive reinforcement
Injury prevention suggestions

Streaming responses provide an interactive coaching experience.

4. Webcam Pose Detection

Powered by MediaPipe Pose.

Features:

33 body landmarks
Local browser inference
Automatic joint angle extraction
45 FPS posture analysis
Privacy-first processing
5. Progress Dashboard

Track improvement over time.

Includes:

Good vs Bad rep charts
Streak tracking
Weekly performance summaries
Fault frequency analysis

Example:

Knee Cave: 14 occurrences
Excessive Spine Tilt: 9 occurrences
6. Workout Plan Generator

Generate AI-powered workout plans based on:

Goal
Equipment availability
Weekly schedule

Provides:

Exercise selection
Sets
Reps
Rest periods
Weekly structure
7. Rep Counter

Automatic repetition counting using range-of-motion tracking.

Features:

Threshold crossing detection
Bottom position validation
Good-form rep verification

Only quality repetitions are counted.

8. Form History Log

Complete training history storage.

Stores:

Timestamp
Exercise
Rep count
Good/Bad ratio
Coaching feedback

Export data as CSV for analysis.

9. Custom Exercise Profiles

Create personalized exercise definitions.

Configure:

Joint angle targets
Acceptable ranges
Exercise-specific thresholds
Classification sensitivity

Combines:

Rule-based validation
Machine-learning predictions
10. Injury Risk Alerts

Detect potentially harmful movement patterns.

Triggers alerts when:

Extreme angle violations occur
Multiple bad reps happen consecutively
Fatigue-related breakdown is detected

Provides:

AI-generated risk explanation
Recommended modifications
Recovery suggestions
11. AI Nutrition & Balanced Diet Recommendation

Generate personalized nutrition plans based on:

Exercise performance
Training volume
Fitness goals
Recovery indicators
Injury risk patterns

Outputs:

Daily calorie target
Protein recommendation
Carb and fat distribution
Meal suggestions
Recovery nutrition advice

Example Goals:

Strength
Muscle Gain
Weight Loss
Mobility
General Fitness
Technology Stack
Layer	Technology
Frontend	React
Styling	Tailwind CSS
Pose Detection	MediaPipe Pose
Machine Learning	TensorFlow.js / Brain.js
AI Coaching	Anthropic Claude Sonnet
Charts	Recharts
Data Storage	localStorage
CSV Handling	PapaParse
Training Data Format
knee_angle_l,knee_angle_r,hip_angle,spine_tilt,knee_over_toe,shoulder_sym,label
92,91,88,3,1.01,0.98,1
93,90,87,4,1.02,0.97,1
112,108,102,18,1.4,0.85,0
95,115,90,22,1.35,0.79,0
88,89,86,2,0.99,0.99,1

Label:

1 = Good Form
0 = Bad Form
Privacy
Pose detection runs entirely in-browser.
No webcam frames are uploaded.
Model training occurs locally.
User data remains under user control.
Only coaching and plan-generation requests are sent to the AI API.
Future Enhancements
Multi-person tracking
Mobile app support
Wearable device integration
Voice coaching
Exercise auto-detection
Nutrition tracking
Macro compliance scoring
Weekly progress reports
License

MIT License
