# Flutter Exam Notes - Theory Focused Guide

**Exam Date: November 2, 2025**

---

## 1. FLUTTER – INTRODUCTION

### What is Flutter?
Flutter is a **free and open-source UI software development toolkit** created by **Google**. It is used to build beautiful, natively compiled applications for **mobile, web, and desktop** from a **single codebase**. Flutter was first released in 2017 and has become one of the most popular frameworks for cross-platform development.

### Key Points:
- **Creator**: Google
- **Release Year**: 2017
- **Language**: Dart programming language
- **Purpose**: Build apps for multiple platforms using one codebase
- **Type**: UI Framework (User Interface Framework)

### Features of Flutter

#### 1. **Cross-Platform Development**
- Write code once and deploy it on multiple platforms (Android, iOS, Web, Windows, macOS, Linux)
- Saves time and resources
- Maintains consistent look across all platforms

#### 2. **Hot Reload**
- Allows developers to see changes **immediately** without restarting the app
- Makes development **faster and more productive**
- State of the app is preserved during reload
- Helps in quick bug fixing and UI experiments

#### 3. **Beautiful and Customizable UI**
- Provides rich set of **pre-designed widgets**
- Widgets follow **Material Design** (Google's design) and **Cupertino** (Apple's design)
- Highly customizable to create unique designs
- Smooth animations and transitions

#### 4. **Native Performance**
- Apps compiled to **native machine code**
- No JavaScript bridge (unlike React Native)
- Direct communication with platform
- Fast rendering at **60 FPS** (frames per second) or **120 FPS** on capable devices

#### 5. **Single Codebase**
- One code for all platforms
- Reduces development time by almost 50%
- Easier to maintain and update
- Consistent business logic across platforms

#### 6. **Own Rendering Engine**
- Uses **Skia graphics library** (also used by Chrome and Android)
- Draws its own UI instead of using platform widgets
- Ensures **consistent UI** across all platforms
- Complete control over every pixel on screen

#### 7. **Widget-Based Architecture**
- Everything in Flutter is a **widget**
- Widgets are building blocks of UI
- Easy to understand and use
- Reusable components

#### 8. **Rich Development Tools**
- Flutter DevTools for debugging
- Hot reload and hot restart
- Widget inspector to visualize widget tree
- Performance profiling tools

### Advantages of Flutter

#### 1. **Faster Development**
- Hot reload feature speeds up development
- Single codebase reduces development time
- Rich widget library saves coding time
- Easy to learn and implement

#### 2. **Cost Effective**
- One team can build for all platforms
- Less development time = less cost
- Single codebase = reduced maintenance cost
- Fewer resources needed

#### 3. **Excellent Performance**
- Compiled to native code
- No performance bridge
- Smooth 60 FPS animations
- Fast startup time

#### 4. **Beautiful and Consistent UI**
- Pre-built widgets for common UI elements
- Customizable designs
- Same look on all devices
- Modern and attractive interfaces

#### 5. **Growing Community**
- Large community of developers
- Many packages and plugins available
- Good documentation
- Easy to find solutions to problems

#### 6. **Strong Backing**
- Supported by Google
- Used by big companies (Alibaba, BMW, Google Ads)
- Regular updates and improvements
- Long-term support guaranteed

#### 7. **Easy Testing**
- Write tests once for all platforms
- Good testing tools available
- Widget testing, unit testing, integration testing
- Saves testing time and effort

#### 8. **Great Documentation**
- Well-documented framework
- Many tutorials and examples
- Active community support
- Easy for beginners

### Disadvantages of Flutter

#### 1. **Large App Size**
- Flutter apps are **larger in size** compared to native apps
- Minimum app size is around 4-6 MB even for simple apps
- Includes Flutter engine and framework code
- Can be a problem for users with limited storage

#### 2. **Relatively New**
- Launched in 2017, still newer than other frameworks
- Fewer third-party libraries compared to native development
- Some advanced features may not be available yet
- Still evolving and changing

#### 3. **Learning Curve for Dart**
- Uses Dart language which is **less popular** than JavaScript or Java
- Developers need to learn new language
- Smaller Dart community compared to JavaScript
- Fewer learning resources for Dart

#### 4. **Limited Libraries**
- Fewer ready-made packages compared to native platforms
- Some specific functionalities may require custom development
- Not all native features have Flutter packages yet
- May need to write platform-specific code for some features

#### 5. **Platform-Specific Features**
- Delay in supporting latest iOS/Android features
- Need to wait for Flutter team to add support
- Sometimes requires writing native code
- May not support all device-specific features

#### 6. **Limited IDE Support**
- Mainly supported in Android Studio and VS Code
- Not as many development tools as native development
- Some IDEs have limited Flutter support

#### 7. **Continuous Updates**
- Frequent updates can break existing code
- Need to keep updating the app
- May require code changes after Flutter updates

---

## 2. FLUTTER – INSTALLATION

### System Requirements

#### For Windows:
- **Operating System**: Windows 7 SP1 or later (64-bit)
- **Disk Space**: 2.8 GB (does not include disk space for IDE/tools)
- **Tools Required**: Windows PowerShell, Git for Windows

#### For MacOS:
- **Operating System**: macOS (64-bit)
- **Disk Space**: 2.8 GB (does not include disk space for IDE/tools)
- **Tools Required**: bash, curl, git, unzip, which

### Installation in Windows

#### Step-by-Step Process:

**Step 1: Download Flutter SDK**
- Visit the official Flutter website (flutter.dev)
- Go to "Get Started" section
- Download Flutter SDK for Windows (zip file)
- File size is approximately 1-2 GB

**Step 2: Extract Flutter SDK**
- Extract the downloaded zip file
- Place it in a desired location (Example: C:\flutter)
- **Important**: Don't place in Program Files (requires admin privileges)
- Avoid paths with special characters or spaces

**Step 3: Update System PATH**
- PATH is an environment variable that tells Windows where to find programs
- Add Flutter to PATH so you can run Flutter commands from anywhere
- Process:
  - Right-click on "This PC" → Properties
  - Click "Advanced system settings"
  - Click "Environment Variables"
  - Under "User variables", find "Path"
  - Add new entry: `C:\flutter\bin` (or your installation path)
  - Click OK to save

**Step 4: Run Flutter Doctor**
- Open Command Prompt or PowerShell
- Type: `flutter doctor`
- This command checks your environment and shows what needs to be set up
- It identifies missing dependencies

**Step 5: Install Android Studio**
- Required for Android app development
- Download from developer.android.com/studio
- Install Android SDK, Android SDK Platform, and Android Virtual Device
- Install Flutter and Dart plugins in Android Studio

**Step 6: Install IDE (Optional)**
- Install Visual Studio Code (lightweight option)
- Install Flutter and Dart extensions in VS Code
- Or continue using Android Studio (full-featured option)

### Installation in MacOS

#### Step-by-Step Process:

**Step 1: Download Flutter SDK**
- Visit flutter.dev
- Download Flutter SDK for macOS
- Choose appropriate version (Intel or Apple Silicon)

**Step 2: Extract Flutter SDK**
- Extract the zip file
- Place in home directory or another location
- Example: /Users/username/development/flutter

**Step 3: Update PATH Variable**
- Open Terminal
- Edit bash profile or zsh profile
- For bash: `nano ~/.bash_profile`
- For zsh: `nano ~/.zshrc`
- Add Flutter to PATH
- Save and close file
- Run: `source ~/.bash_profile` or `source ~/.zshrc`
- This makes Flutter commands available system-wide

**Step 4: Run Flutter Doctor**
- Open Terminal
- Type: `flutter doctor`
- Check all requirements
- Follow instructions to fix any issues

**Step 5: Install Xcode**
- Required for iOS app development
- Download from Mac App Store
- Install Xcode Command Line Tools
- Accept Xcode license agreement
- Configure Xcode for first use

**Step 6: Install Android Studio**
- Required for Android development
- Download and install Android Studio
- Install Android SDK
- Install Flutter and Dart plugins

**Step 7: Setup iOS Simulator**
- Open Xcode
- Install iOS Simulator
- Or connect physical iOS device for testing

### Flutter Doctor Command

**What is Flutter Doctor?**
- A diagnostic tool that checks Flutter installation
- Verifies all required dependencies
- Shows what's missing or needs configuration
- Provides solution suggestions

**What It Checks:**
1. **Flutter SDK**: Whether Flutter is properly installed
2. **Android toolchain**: Android Studio, SDK, licenses
3. **Xcode** (macOS only): For iOS development
4. **Chrome**: For web development
5. **Android Studio**: IDE and plugins
6. **VS Code**: Alternative IDE and plugins
7. **Connected devices**: Available devices for testing

**Common Issues and Solutions:**
- Missing Android licenses: Run `flutter doctor --android-licenses`
- Xcode not configured: Open Xcode and accept license
- No devices available: Start emulator or connect device
- IDE plugins missing: Install Flutter and Dart plugins

### Additional Setup

**For Android Development:**
- Install Java Development Kit (JDK)
- Configure Android SDK
- Accept Android licenses
- Create Android Virtual Device (AVD) for testing

**For iOS Development (macOS only):**
- Install Xcode
- Install CocoaPods (dependency manager)
- Setup iOS Simulator
- Configure signing certificates for physical devices

**For Web Development:**
- Install Chrome browser
- Enable web support: `flutter config --enable-web`

**For Desktop Development:**
- Enable desktop support for Windows/macOS/Linux
- Install platform-specific requirements

---

## 3. FLUTTER – CREATING SIMPLE APPLICATION IN ANDROID STUDIO

### Understanding Flutter Project Creation

### Steps to Create Your First App in Android Studio:

**Step 1: Open Android Studio**
- Launch Android Studio on your computer
- Wait for it to fully load
- Make sure Flutter and Dart plugins are installed

**Step 2: Start New Flutter Project**
- Click on "New Flutter Project" from welcome screen
- Or go to File → New → New Flutter Project
- Select "Flutter Application" as project type
- Click "Next"

**Step 3: Configure Project**
- **Project Name**: Enter a name (use lowercase with underscores, e.g., my_first_app)
- **Flutter SDK Path**: Specify where Flutter is installed
- **Project Location**: Choose where to save the project
- **Description**: Optional description of your app

**Step 4: Set Project Details**
- **Organization**: Your company domain in reverse (e.g., com.example)
- **Platform Languages**: 
  - Android: Java or Kotlin
  - iOS: Objective-C or Swift
- Click "Finish"

**Step 5: Wait for Project Creation**
- Android Studio creates project structure
- Downloads required dependencies
- This may take a few minutes
- Status shown in bottom of Android Studio

### Understanding Flutter Project Structure

#### Main Folders and Files:

**1. lib/ folder**
- Contains all Dart code
- Main application logic resides here
- `main.dart` is the entry point of the app
- Most of your coding happens in this folder

**2. android/ folder**
- Contains Android-specific code
- Android native project files
- Used when you need to write Android-specific features
- Contains AndroidManifest.xml (app permissions, configurations)

**3. ios/ folder**
- Contains iOS-specific code
- iOS native project files
- Used for iOS-specific features
- Contains Info.plist (iOS configurations)

**4. test/ folder**
- Contains test files
- Write unit tests here
- Helps ensure code works correctly
- Tests run separately from main app

**5. pubspec.yaml file**
- Most important configuration file
- Defines app metadata (name, version, description)
- Lists all dependencies (packages your app needs)
- Specifies assets (images, fonts, files)
- Written in YAML format (key: value pairs)

**6. assets/ folder**
- Stores static files (images, fonts, JSON files)
- Must be declared in pubspec.yaml
- Accessible in app code
- Not created by default, you create it when needed

**7. build/ folder**
- Contains compiled code
- Generated automatically when you run the app
- Can be deleted; will regenerate
- Don't manually edit this folder

### Key Components of a Flutter App

#### 1. **main() Function**
- The **starting point** of every Flutter app
- First function that runs when app launches
- Calls runApp() function
- Located in lib/main.dart file
- Required in every Flutter application

#### 2. **runApp() Function**
- Takes a widget as parameter
- Inflates (displays) the given widget
- Makes it the root of the widget tree
- Called from main() function
- Starts the Flutter framework

#### 3. **MaterialApp Widget**
- The root widget of your application
- Provides Material Design styling
- Configures app-wide settings
- Contains properties like:
  - **title**: App name shown in task manager
  - **theme**: App-wide color and style settings
  - **home**: The first screen users see
  - **routes**: For navigation between screens

#### 4. **Scaffold Widget**
- Provides basic visual layout structure
- Implements the basic Material Design layout
- Has predefined slots for common UI elements
- Contains properties like:
  - **appBar**: Top bar with title
  - **body**: Main content area
  - **floatingActionButton**: Floating button (like + button)
  - **drawer**: Side navigation menu
  - **bottomNavigationBar**: Bottom navigation

#### 5. **AppBar Widget**
- The top bar of your app
- Shows app title and actions
- Can contain icons and menu buttons
- Properties include:
  - **title**: Text or widget for title
  - **actions**: List of icon buttons
  - **backgroundColor**: Color of the app bar
  - **elevation**: Shadow depth

#### 6. **Body**
- Main content area of the screen
- Can contain any widget
- Usually contains Center, Column, Row, ListView, etc.
- This is where your main UI goes

#### 7. **Text Widget**
- Displays text on screen
- Can be styled with different fonts, sizes, colors
- Most basic and commonly used widget

#### 8. **Center Widget**
- Centers its child widget
- Positions widget in the middle of available space
- Useful for centering content

### Running Your First App

**Step 1: Select Device**
- Click on device dropdown in toolbar
- Choose Android Emulator, iOS Simulator, or physical device
- If no device available, create Android Virtual Device (AVD)

**Step 2: Run the App**
- Click green play button (Run)
- Or press Shift + F10 (Windows/Linux) or Control + R (Mac)
- App compiles and installs on selected device
- First run takes longer (subsequent runs are faster)

**Step 3: See Your App**
- App opens on device/emulator
- Shows default Flutter counter app
- Has + button that increments counter
- Demonstrates basic interactivity

**Step 4: Make Changes**
- Edit code in main.dart
- Change text or colors
- Save file
- Use Hot Reload (lightning icon) to see changes instantly

### Hot Reload vs Hot Restart

**Hot Reload:**
- Quick update (keyboard: 'r')
- Takes 1-2 seconds
- Preserves app state
- Only updates changed code
- Best for UI changes

**Hot Restart:**
- Full restart (keyboard: 'R')
- Takes longer (5-10 seconds)
- Resets app state to initial
- Reloads all code
- Use when hot reload doesn't work

### Understanding the Default Counter App

The default app Flutter creates has:
- A counter variable (number)
- A text showing counter value
- A + button to increase counter
- Demonstrates StatefulWidget (changeable state)
- Shows basic app structure and interactivity

**Main concepts demonstrated:**
1. State management (how data changes)
2. Event handling (button press)
3. UI updates (showing new counter value)
4. Basic layout (AppBar, Body, Button)

---

## 4. FLUTTER – ARCHITECTURE OF FLUTTER APPLICATION

### Understanding Flutter Architecture

Flutter has a **layered architecture** designed for flexibility and performance. Understanding this architecture is crucial for building efficient apps.

### Four Main Components:

### 1. Widgets - The Building Blocks

**What are Widgets?**
- Widgets are the **fundamental building blocks** of Flutter UI
- Everything you see on screen is a widget
- **"Everything is a Widget"** is Flutter's core philosophy
- Widgets describe what their view should look like

**Characteristics of Widgets:**
- **Immutable**: Once created, widgets cannot be changed
- **Lightweight**: Widgets are temporary objects
- **Declarative**: You describe what you want, Flutter figures out how to do it
- **Composable**: Small widgets combine to make complex UIs

**Types of Widgets:**

**A. StatelessWidget**
- Widgets that **don't change** over time
- Static and immutable
- No internal state to manage
- Examples: Text, Icon, Image displaying fixed content
- **When to use**: When widget doesn't need to track changing information
- More efficient because they don't rebuild unnecessarily
- Example scenarios: Static labels, icons, images

**B. StatefulWidget**
- Widgets that **can change** over time
- Dynamic and mutable
- Maintain state that can change
- Examples: Checkbox, TextField, Counter, Form inputs
- **When to use**: When widget needs to track and display changing data
- Rebuilds when state changes
- Example scenarios: User input, animations, data from server

**Widget Tree:**
- Widgets are organized in a **hierarchical tree structure**
- Parent widgets contain child widgets
- Tree starts from root widget (usually MaterialApp)
- Efficient for rebuilding only changed parts

**Widget Lifecycle:**
- Widgets are created, built, and destroyed
- Flutter manages this lifecycle automatically
- StatefulWidget has longer lifecycle with multiple states

### 2. Gestures - User Interactions

**What are Gestures?**
- Gestures are **user interactions** with the screen
- How users communicate with your app
- Touch, tap, drag, swipe, pinch, etc.

**Types of Gestures:**

**A. Tap Gestures**
- **Single Tap (onTap)**: Quick touch and release
- **Double Tap (onDoubleTap)**: Two quick taps
- **Long Press (onLongPress)**: Touch and hold
- Most common user interaction

**B. Drag Gestures**
- **Pan**: Moving finger across screen
- **Swipe**: Quick drag motion
- Used for scrolling, moving objects

**C. Scale Gestures**
- **Pinch**: Two fingers moving together or apart
- Used for zooming in/out
- Common in maps and image viewers

**Gesture Detection:**
- Flutter provides **GestureDetector** widget
- Wraps other widgets to make them interactive
- Detects and responds to gestures
- Can detect multiple gesture types simultaneously

**Gesture Priority:**
- When multiple gestures possible, Flutter resolves conflicts
- More specific gestures take priority
- Gesture arena determines winner

### 3. Concept of State - Managing Data

**What is State?**
- **State** is information that can be read when widget is built
- Data that **changes over time**
- When state changes, UI rebuilds to reflect changes
- Core concept for interactive apps

**Why State Matters:**
- Apps need to respond to user actions
- Data changes based on events
- UI must reflect current data
- State management keeps UI synchronized with data

**Types of State:**

**A. Ephemeral State (Local State)**
- State needed by **single widget or small group**
- Short-lived and local
- Not shared with other parts of app
- Managed using setState() in StatefulWidget
- Examples: Current page in PageView, animation progress, form input values
- **Scope**: Limited to one widget

**B. App State (Global State)**
- State needed by **many parts of the app**
- Shared across multiple screens
- Lives longer than ephemeral state
- Requires state management solution
- Examples: User login info, shopping cart, user preferences, theme settings
- **Scope**: Entire application or major sections

**State Management Principles:**
- Keep state as local as possible
- Lift state up when multiple widgets need it
- Use appropriate state management for app size
- Separate UI from business logic

**setState() Method:**
- Special method in StatefulWidget
- Tells Flutter that state has changed
- Triggers widget rebuild
- Updates UI with new state
- Called inside State class

**State Management Solutions:**
- **Provider**: Popular, recommended by Flutter team
- **Bloc**: Business Logic Component pattern
- **GetX**: Lightweight and powerful
- **Riverpod**: Improved Provider
- **setState**: Built-in, for simple cases

### 4. Layers - Architecture Layers

Flutter architecture consists of **three main layers**:

**Layer 1: Framework Layer (Dart)**
- **Top layer** - What developers interact with
- Written entirely in **Dart language**
- Contains all widgets and APIs
- Includes:
  - **Widgets**: Building blocks
  - **Rendering**: Layout and painting logic
  - **Animation**: Animation framework
  - **Gestures**: Touch and interaction handling
  - **Foundation**: Basic building blocks
- Most developer work happens here
- High-level, easy to use APIs

**Layer 2: Engine Layer (C/C++)**
- **Middle layer** - Core of Flutter
- Written in **C and C++** for performance
- Handles:
  - **Rendering**: Uses Skia graphics library
  - **Text Layout**: Displaying text
  - **Dart Runtime**: Executes Dart code
  - **Platform Channels**: Communication with native code
  - **Accessibility**: Support for accessibility features
- Developers rarely interact directly
- Provides low-level implementations
- Ensures high performance

**Layer 3: Platform Layer (Embedder)**
- **Bottom layer** - Platform specific
- Different for each platform (Android, iOS, Windows, etc.)
- Provides:
  - **Platform API Access**: Camera, GPS, sensors
  - **Event Loop**: Processes events
  - **Rendering Surface**: Where UI is drawn
  - **Plugin APIs**: For native features
- Written in platform language (Java/Kotlin for Android, Swift/Objective-C for iOS)
- Allows Flutter to run on different platforms

**How Layers Work Together:**
1. You write code using Framework Layer (Dart)
2. Framework Layer communicates with Engine Layer
3. Engine Layer renders UI and talks to Platform Layer
4. Platform Layer provides native capabilities
5. Result: Beautiful, fast, cross-platform apps

**Benefits of Layered Architecture:**
- **Separation of Concerns**: Each layer has specific responsibility
- **Flexibility**: Can work at appropriate abstraction level
- **Performance**: Low-level layers optimized for speed
- **Portability**: Easy to add new platforms
- **Maintainability**: Clear structure makes updates easier

### Widget Build Process

**How Flutter Builds UI:**

**Step 1: Widget Tree**
- You create widgets in code
- Widgets form hierarchical tree
- Immutable description of UI

**Step 2: Element Tree**
- Flutter creates element for each widget
- Elements are mutable, persist across builds
- Link between widgets and rendering

**Step 3: Render Tree**
- Elements create render objects
- Render objects do actual layout and painting
- Handle size, position, and painting logic

**Step 4: Display**
- Render objects paint to screen
- Skia engine handles low-level rendering
- Result: Beautiful UI on screen

**Rebuild Process:**
- When state changes, only affected widgets rebuild
- Flutter compares old and new widget trees
- Only updates what changed
- Very efficient and fast

### Platform Channels

**What are Platform Channels?**
- Communication bridge between Flutter and native platform
- Allows calling platform-specific code
- Used when Flutter doesn't have built-in support

**Types of Channels:**
- **MethodChannel**: Call methods and get results
- **EventChannel**: Stream of events from platform
- **BasicMessageChannel**: Simple message passing

**Use Cases:**
- Accessing device hardware (camera, GPS, battery)
- Using platform-specific APIs
- Integrating existing native code
- Features not yet in Flutter

**How It Works:**
- Flutter code sends message through channel
- Platform receives and processes message
- Platform sends response back
- Flutter receives and uses response

---

## 5. DART PROGRAMMING BASICS

### Variables and Data Types

**Variables:**
```dart
var name = "John";           // Auto type
String name = "John";        // String type
int age = 25;                // Integer
double price = 99.99;        // Decimal
bool isStudent = true;       // Boolean
```

**Data Types:**
- `int` - Whole numbers (1, 2, 100)
- `double` - Decimal numbers (3.14, 99.99)
- `String` - Text ("Hello")
- `bool` - True or False
- `List` - Collection of items [1, 2, 3]
- `Map` - Key-value pairs {"name": "John"}

### Decision Making and Loops

**If-Else:**
```dart
if (age >= 18) {
  print("Adult");
} else {
  print("Child");
}
```

**For Loop:**
```dart
for (int i = 0; i < 5; i++) {
  print(i);
}
```

**While Loop:**
```dart
while (count < 10) {
  print(count);
  count++;
}
```

### Functions
```dart
// Simple function
void greet() {
  print("Hello!");
}

// Function with parameters
String sayHello(String name) {
  return "Hello, $name!";
}

// Function with named parameters
void createUser({String name, int age}) {
  print("$name is $age years old");
}
```

### Object Oriented Programming

**Class:**
```dart
class Person {
  String name;
  int age;
  
  // Constructor
  Person(this.name, this.age);
  
  // Method
  void introduce() {
    print("I am $name, $age years old");
  }
}

// Using the class
Person p = Person("John", 25);
p.introduce();
```

**Key OOP Concepts:**
- **Class** - Blueprint for objects
- **Object** - Instance of a class
- **Constructor** - Initializes object
- **Inheritance** - Class extends another class
- **Encapsulation** - Data hiding

---

## 6. INTRODUCTION TO WIDGETS

### Two Types of Widgets:

#### 1. StatelessWidget
- **Cannot change** once created
- Used for static content
- Example: Text, Icon, Image

```dart
class MyWidget extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Text("I don't change!");
  }
}
```

#### 2. StatefulWidget
- **Can change** over time
- Used for dynamic content
- Example: Checkbox, TextField, Counter

```dart
class MyWidget extends StatefulWidget {
  @override
  _MyWidgetState createState() => _MyWidgetState();
}

class _MyWidgetState extends State<MyWidget> {
  int counter = 0;
  
  @override
  Widget build(BuildContext context) {
    return Text("Counter: $counter");
  }
}
```

### Common Widgets:

**Text Widget:**
```dart
Text('Hello World')
```

**Image Widget:**
```dart
Image.network('https://example.com/image.jpg')
Image.asset('assets/image.png')
```

**Button Widgets:**
```dart
ElevatedButton(
  onPressed: () { print("Clicked!"); },
  child: Text("Click Me"),
)

TextButton(...)
IconButton(...)
```

**Container Widget:**
```dart
Container(
  width: 100,
  height: 100,
  color: Colors.blue,
  child: Text("Box"),
)
```

---

## 7. INTRODUCTION TO LAYOUTS

### Types of Layout Widgets:

### A. Single Child Widgets
**Can have only ONE child**

#### 1. Container
- Like a box to hold widgets
```dart
Container(
  width: 200,
  height: 100,
  padding: EdgeInsets.all(10),
  margin: EdgeInsets.all(20),
  decoration: BoxDecoration(
    color: Colors.blue,
    borderRadius: BorderRadius.circular(10),
  ),
  child: Text("Hello"),
)
```

#### 2. Center
- Centers the child widget
```dart
Center(
  child: Text("I'm centered!"),
)
```

#### 3. Padding
- Adds space around child
```dart
Padding(
  padding: EdgeInsets.all(16.0),
  child: Text("Padded text"),
)
```

#### 4. Align
- Aligns child in specific position
```dart
Align(
  alignment: Alignment.topRight,
  child: Text("Top Right"),
)
```

### B. Multiple Child Widgets
**Can have multiple children**

#### 1. Row
- Arranges children **horizontally** (left to right)
```dart
Row(
  children: [
    Icon(Icons.star),
    Text("Rating"),
    Icon(Icons.star),
  ],
)
```

#### 2. Column
- Arranges children **vertically** (top to bottom)
```dart
Column(
  children: [
    Text("Line 1"),
    Text("Line 2"),
    Text("Line 3"),
  ],
)
```

#### 3. Stack
- Overlaps children on top of each other
```dart
Stack(
  children: [
    Image.network('background.jpg'),
    Text("Text on image"),
  ],
)
```

#### 4. ListView
- Scrollable list of children
```dart
ListView(
  children: [
    ListTile(title: Text("Item 1")),
    ListTile(title: Text("Item 2")),
    ListTile(title: Text("Item 3")),
  ],
)
```

#### 5. GridView
- Grid layout (like a photo gallery)
```dart
GridView.count(
  crossAxisCount: 2,
  children: [
    Container(color: Colors.red),
    Container(color: Colors.blue),
    Container(color: Colors.green),
  ],
)
```

### Important Properties:
- **mainAxisAlignment** - Alignment along main axis
- **crossAxisAlignment** - Alignment along cross axis
- **children** - List of child widgets

---

## 8. INTRODUCTION TO GESTURES

### What are Gestures?
Gestures are user interactions with the screen (tap, swipe, drag, etc.)

### Common Gestures:

#### 1. GestureDetector
Most common widget for handling gestures

```dart
GestureDetector(
  onTap: () {
    print("Tapped!");
  },
  onDoubleTap: () {
    print("Double tapped!");
  },
  onLongPress: () {
    print("Long pressed!");
  },
  child: Container(
    width: 100,
    height: 100,
    color: Colors.blue,
  ),
)
```

### Types of Gestures:
1. **onTap** - Single tap
2. **onDoubleTap** - Double tap
3. **onLongPress** - Press and hold
4. **onPanUpdate** - Drag/Swipe
5. **onScaleUpdate** - Pinch to zoom

### InkWell
- Similar to GestureDetector but with ripple effect
```dart
InkWell(
  onTap: () {
    print("Tapped with ripple!");
  },
  child: Container(
    padding: EdgeInsets.all(12),
    child: Text("Click Me"),
  ),
)
```

---

## 9. STATE MANAGEMENT

### What is State?
**State** = Data that can change and affect the UI

### Types of State:

### 1. Ephemeral State (Local State)
- State used in single widget
- Use **setState()**

**Example - Counter App:**
```dart
class CounterApp extends StatefulWidget {
  @override
  _CounterAppState createState() => _CounterAppState();
}

class _CounterAppState extends State<CounterApp> {
  int counter = 0;  // This is state
  
  void increment() {
    setState(() {
      counter++;  // Update state
    });
  }
  
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      body: Center(
        child: Text('Count: $counter'),
      ),
      floatingActionButton: FloatingActionButton(
        onPressed: increment,
        child: Icon(Icons.add),
      ),
    );
  }
}
```

**Key Points:**
- Use **StatefulWidget** for changeable data
- Use **setState()** to update UI
- State is private to the widget

### 2. Application State (Global State)
- State shared across multiple screens
- Use packages like **scoped_model**, **Provider**, **Bloc**

**Using scoped_model:**
```dart
// 1. Create a model
class CounterModel extends Model {
  int counter = 0;
  
  void increment() {
    counter++;
    notifyListeners();  // Notify all listeners
  }
}

// 2. Wrap app with ScopedModel
ScopedModel<CounterModel>(
  model: CounterModel(),
  child: MyApp(),
)

// 3. Use the model
ScopedModelDescendant<CounterModel>(
  builder: (context, child, model) {
    return Text('${model.counter}');
  },
)
```

### Navigation and Routing

**Navigate to new screen:**
```dart
// Push new screen
Navigator.push(
  context,
  MaterialPageRoute(builder: (context) => SecondScreen()),
);

// Go back
Navigator.pop(context);
```

**Named Routes:**
```dart
// Define routes
MaterialApp(
  routes: {
    '/': (context) => HomeScreen(),
    '/second': (context) => SecondScreen(),
  },
);

// Navigate using names
Navigator.pushNamed(context, '/second');
```

**Pass data between screens:**
```dart
// Send data
Navigator.push(
  context,
  MaterialPageRoute(
    builder: (context) => DetailScreen(data: "Hello"),
  ),
);

// Receive data
class DetailScreen extends StatelessWidget {
  final String data;
  DetailScreen({this.data});
  
  @override
  Widget build(BuildContext context) {
    return Text(data);
  }
}
```

---

## 10. ANIMATION

### What is Animation?
Animation makes your app more **interactive and beautiful** by moving or changing widgets smoothly.

### Animation Classes:

#### 1. Animation
- Represents the value that changes over time
- Example: 0 to 1, 0 to 100

#### 2. AnimationController
- Controls the animation (start, stop, repeat)
```dart
AnimationController controller = AnimationController(
  duration: Duration(seconds: 2),
  vsync: this,
);
```

#### 3. Tween
- Defines start and end values
```dart
Tween<double>(begin: 0.0, end: 300.0)
```

#### 4. Curve
- Defines animation speed (slow start, fast end, etc.)
```dart
CurvedAnimation(
  parent: controller,
  curve: Curves.easeInOut,
)
```

### Animation Workflow:
1. Create **AnimationController**
2. Define **Tween** (start and end values)
3. Create **Animation** object
4. Use **setState()** or **AnimatedBuilder** to rebuild
5. **Start** animation

### Simple Animation Example:
```dart
class MyAnimation extends StatefulWidget {
  @override
  _MyAnimationState createState() => _MyAnimationState();
}

class _MyAnimationState extends State<MyAnimation> 
    with SingleTickerProviderStateMixin {
  
  AnimationController controller;
  Animation<double> animation;
  
  @override
  void initState() {
    super.initState();
    
    // Create controller
    controller = AnimationController(
      duration: Duration(seconds: 2),
      vsync: this,
    );
    
    // Create animation
    animation = Tween<double>(begin: 0, end: 300).animate(controller);
    
    // Start animation
    controller.forward();
  }
  
  @override
  Widget build(BuildContext context) {
    return AnimatedBuilder(
      animation: animation,
      builder: (context, child) {
        return Container(
          width: animation.value,
          height: animation.value,
          color: Colors.blue,
        );
      },
    );
  }
  
  @override
  void dispose() {
    controller.dispose();
    super.dispose();
  }
}
```

### Built-in Animated Widgets:
- **AnimatedContainer** - Animates size, color, etc.
- **AnimatedOpacity** - Fade in/out
- **Hero** - Animate between screens

---

## 11. WRITING ANDROID SPECIFIC CODE

### Platform Channel
Used to call **Android (Java/Kotlin)** code from Flutter

### Steps:
1. **Flutter Side** - Call platform method
2. **Android Side** - Write native code
3. **Communication** - Use MethodChannel

### Flutter Side (Dart):
```dart
import 'package:flutter/services.dart';

class BatteryLevel {
  static const platform = MethodChannel('samples.flutter.dev/battery');
  
  Future<String> getBatteryLevel() async {
    try {
      final int result = await platform.invokeMethod('getBatteryLevel');
      return 'Battery level: $result%';
    } catch (e) {
      return 'Failed to get battery level';
    }
  }
}
```

### Android Side (Kotlin):
```kotlin
// In MainActivity.kt
private val CHANNEL = "samples.flutter.dev/battery"

override fun configureFlutterEngine(flutterEngine: FlutterEngine) {
    MethodChannel(flutterEngine.dartExecutor.binaryMessenger, CHANNEL)
        .setMethodCallHandler { call, result ->
            if (call.method == "getBatteryLevel") {
                val batteryLevel = getBatteryLevel()
                result.success(batteryLevel)
            } else {
                result.notImplemented()
            }
        }
}

private fun getBatteryLevel(): Int {
    val batteryManager = getSystemService(Context.BATTERY_SERVICE) as BatteryManager
    return batteryManager.getIntProperty(BatteryManager.BATTERY_PROPERTY_CAPACITY)
}
```

**Use Cases:**
- Access device features (Battery, Camera, GPS)
- Use Android-specific libraries
- Custom native functionality

---

## 12. WRITING iOS SPECIFIC CODE

### Similar to Android, but for iOS (Swift/Objective-C)

### Flutter Side (Dart):
Same as Android - use MethodChannel

### iOS Side (Swift):
```swift
// In AppDelegate.swift
import UIKit
import Flutter

@UIApplicationMain
@objc class AppDelegate: FlutterAppDelegate {
  override func application(
    _ application: UIApplication,
    didFinishLaunchingWithOptions launchOptions: [UIApplication.LaunchOptionsKey: Any]?
  ) -> Bool {
    
    let controller = window?.rootViewController as! FlutterViewController
    let batteryChannel = FlutterMethodChannel(
        name: "samples.flutter.dev/battery",
        binaryMessenger: controller.binaryMessenger
    )
    
    batteryChannel.setMethodCallHandler { (call, result) in
      if call.method == "getBatteryLevel" {
        self.receiveBatteryLevel(result: result)
      } else {
        result(FlutterMethodNotImplemented)
      }
    }
    
    return super.application(application, didFinishLaunchingWithOptions: launchOptions)
  }
  
  private func receiveBatteryLevel(result: FlutterResult) {
    let device = UIDevice.current
    device.isBatteryMonitoringEnabled = true
    let batteryLevel = Int(device.batteryLevel * 100)
    result(batteryLevel)
  }
}
```

---

## 13. INTRODUCTION TO PACKAGES

### What are Packages?
Packages are **reusable code libraries** that add functionality to your app.

### Types of Packages:

#### 1. Dart Packages
- Pure Dart code only
- Works on all platforms
- Example: http, intl, path

#### 2. Plugin Packages
- Contains both Dart and native code (Android/iOS)
- Platform-specific features
- Example: camera, location, firebase

### Using a Package:

**Steps:**
1. **Find package** on pub.dev
2. **Add to pubspec.yaml**:
```yaml
dependencies:
  flutter:
    sdk: flutter
  http: ^0.13.0  # Add package here
```
3. **Run** `flutter pub get`
4. **Import** in your code:
```dart
import 'package:http/http.dart' as http;
```
5. **Use** the package:
```dart
var response = await http.get(Uri.parse('https://example.com'));
```

### Popular Packages:
- **http** - Make API calls
- **shared_preferences** - Save data locally
- **provider** - State management
- **image_picker** - Pick images
- **sqflite** - Local database
- **firebase** - Backend services

### Develop Your Own Plugin:

**Create plugin:**
```bash
flutter create --template=plugin my_plugin
```

**Structure:**
- `lib/` - Dart code
- `android/` - Android code
- `ios/` - iOS code
- `example/` - Example app

---

## 14. ACCESSING REST API

### Basic Concepts:

**REST API** = Way to communicate with server over internet

**HTTP Methods:**
- **GET** - Fetch data
- **POST** - Send/Create data
- **PUT** - Update data
- **DELETE** - Delete data

### Using http Package:

**1. Add package:**
```yaml
dependencies:
  http: ^0.13.0
```

**2. Import:**
```dart
import 'package:http/http.dart' as http;
import 'dart:convert';
```

**3. GET Request:**
```dart
Future<void> fetchData() async {
  final response = await http.get(
    Uri.parse('https://jsonplaceholder.typicode.com/posts')
  );
  
  if (response.statusCode == 200) {
    // Success
    List data = jsonDecode(response.body);
    print(data);
  } else {
    // Error
    print('Failed to load data');
  }
}
```

**4. POST Request:**
```dart
Future<void> sendData() async {
  final response = await http.post(
    Uri.parse('https://jsonplaceholder.typicode.com/posts'),
    headers: {'Content-Type': 'application/json'},
    body: jsonEncode({
      'title': 'My Post',
      'body': 'This is the content',
      'userId': 1,
    }),
  );
  
  if (response.statusCode == 201) {
    print('Data sent successfully');
  }
}
```

### Complete Example with Model:

**1. Create Model:**
```dart
class Product {
  final int id;
  final String name;
  final double price;
  
  Product({this.id, this.name, this.price});
  
  factory Product.fromJson(Map<String, dynamic> json) {
    return Product(
      id: json['id'],
      name: json['name'],
      price: json['price'],
    );
  }
}
```

**2. Fetch Products:**
```dart
Future<List<Product>> fetchProducts() async {
  final response = await http.get(
    Uri.parse('https://api.example.com/products')
  );
  
  if (response.statusCode == 200) {
    List jsonData = jsonDecode(response.body);
    return jsonData.map((json) => Product.fromJson(json)).toList();
  } else {
    throw Exception('Failed to load products');
  }
}
```

**3. Use in UI:**
```dart
FutureBuilder<List<Product>>(
  future: fetchProducts(),
  builder: (context, snapshot) {
    if (snapshot.hasData) {
      return ListView.builder(
        itemCount: snapshot.data.length,
        itemBuilder: (context, index) {
          return ListTile(
            title: Text(snapshot.data[index].name),
            subtitle: Text('\$${snapshot.data[index].price}'),
          );
        },
      );
    } else if (snapshot.hasError) {
      return Text('Error: ${snapshot.error}');
    }
    return CircularProgressIndicator();
  },
)
```

---

## 15. DATABASE CONCEPTS

### Two Types of Databases:

### 1. SQLite (Local Database)

**What is SQLite?**
- Local database stored on device
- Works offline
- Good for storing app data locally

**Using sqflite package:**

**1. Add package:**
```yaml
dependencies:
  sqflite: ^2.0.0
  path: ^1.8.0
```

**2. Create Database:**
```dart
import 'package:sqflite/sqflite.dart';
import 'package:path/path.dart';

class DatabaseHelper {
  static Database _database;
  
  Future<Database> get database async {
    if (_database != null) return _database;
    _database = await initDatabase();
    return _database;
  }
  
  Future<Database> initDatabase() async {
    String path = join(await getDatabasesPath(), 'my_database.db');
    
    return await openDatabase(
      path,
      version: 1,
      onCreate: (db, version) {
        return db.execute(
          'CREATE TABLE users(id INTEGER PRIMARY KEY, name TEXT, age INTEGER)',
        );
      },
    );
  }
}
```

**3. Insert Data:**
```dart
Future<void> insertUser(Map<String, dynamic> user) async {
  final db = await database;
  await db.insert('users', user);
}
```

**4. Query Data:**
```dart
Future<List<Map<String, dynamic>>> getUsers() async {
  final db = await database;
  return await db.query('users');
}
```

**5. Update Data:**
```dart
Future<void> updateUser(int id, Map<String, dynamic> user) async {
  final db = await database;
  await db.update('users', user, where: 'id = ?', whereArgs: [id]);
}
```

**6. Delete Data:**
```dart
Future<void> deleteUser(int id) async {
  final db = await database;
  await db.delete('users', where: 'id = ?', whereArgs: [id]);
}
```

### 2. Cloud Firestore (Cloud Database)

**What is Cloud Firestore?**
- Google's cloud database
- Real-time synchronization
- Works across devices
- Part of Firebase

**Using Cloud Firestore:**

**1. Setup Firebase** in your project

**2. Add package:**
```yaml
dependencies:
  cloud_firestore: ^3.0.0
```

**3. Add Data:**
```dart
FirebaseFirestore.instance.collection('users').add({
  'name': 'John',
  'age': 25,
});
```

**4. Read Data:**
```dart
StreamBuilder<QuerySnapshot>(
  stream: FirebaseFirestore.instance.collection('users').snapshots(),
  builder: (context, snapshot) {
    if (snapshot.hasData) {
      return ListView(
        children: snapshot.data.docs.map((doc) {
          return ListTile(
            title: Text(doc['name']),
            subtitle: Text('Age: ${doc['age']}'),
          );
        }).toList(),
      );
    }
    return CircularProgressIndicator();
  },
)
```

**5. Update Data:**
```dart
FirebaseFirestore.instance.collection('users').doc(docId).update({
  'age': 26,
});
```

**6. Delete Data:**
```dart
FirebaseFirestore.instance.collection('users').doc(docId).delete();
```

**Comparison:**
| SQLite | Cloud Firestore |
|--------|----------------|
| Local storage | Cloud storage |
| Works offline | Needs internet |
| Free | Paid (free tier available) |
| Manual sync | Auto sync |

---

## 16. INTERNATIONALIZATION (i18n)

### What is Internationalization?
Making your app available in **multiple languages** (English, Hindi, Spanish, etc.)

### Using intl Package:

**Steps:**

**1. Add package:**
```yaml
dependencies:
  flutter_localizations:
    sdk: flutter
  intl: ^0.17.0
```

**2. Add to MaterialApp:**
```dart
import 'package:flutter_localizations/flutter_localizations.dart';

MaterialApp(
  localizationsDelegates: [
    GlobalMaterialLocalizations.delegate,
    GlobalWidgetsLocalizations.delegate,
    GlobalCupertinoLocalizations.delegate,
  ],
  supportedLocales: [
    Locale('en', ''), // English
    Locale('hi', ''), // Hindi
    Locale('es', ''), // Spanish
  ],
  home: MyHomePage(),
)
```

**3. Create translation files:**

**lib/l10n/intl_en.arb** (English):
```json
{
  "title": "Hello World",
  "welcome": "Welcome to Flutter"
}
```

**lib/l10n/intl_hi.arb** (Hindi):
```json
{
  "title": "नमस्ते दुनिया",
  "welcome": "फ्लटर में आपका स्वागत है"
}
```

**4. Use in code:**
```dart
Text(AppLocalizations.of(context).title)
```

### Simple Method - Manual Translation:

```dart
class AppTranslations {
  static Map<String, Map<String, String>> translations = {
    'en': {
      'hello': 'Hello',
      'welcome': 'Welcome',
    },
    'hi': {
      'hello': 'नमस्ते',
      'welcome': 'स्वागत है',
    },
  };
  
  static String translate(String key, String locale) {
    return translations[locale][key] ?? key;
  }
}

// Usage
Text(AppTranslations.translate('hello', 'hi'))
```

---

## 17. TESTING

### Types of Testing:

#### 1. Unit Testing
- Test individual functions
- Fast and simple

#### 2. Widget Testing
- Test individual widgets
- Check if UI works correctly

#### 3. Integration Testing
- Test complete app
- Test user flows

### Widget Testing (Most Common):

**Steps:**

**1. Add test package:**
```yaml
dev_dependencies:
  flutter_test:
    sdk: flutter
```

**2. Create test file:** `test/widget_test.dart`

**3. Write test:**
```dart
import 'package:flutter_test/flutter_test.dart';
import 'package:flutter/material.dart';

void main() {
  testWidgets('Counter increments test', (WidgetTester tester) async {
    // Build the widget
    await tester.pumpWidget(MyApp());
    
    // Verify initial counter is 0
    expect(find.text('0'), findsOneWidget);
    expect(find.text('1'), findsNothing);
    
    // Tap the '+' icon
    await tester.tap(find.byIcon(Icons.add));
    await tester.pump();
    
    // Verify counter incremented
    expect(find.text('0'), findsNothing);
    expect(find.text('1'), findsOneWidget);
  });
}
```

**4. Run test:**
```bash
flutter test
```

### Common Test Functions:
- **expect()** - Check if condition is true
- **find.text()** - Find widget by text
- **find.byIcon()** - Find widget by icon
- **find.byType()** - Find widget by type
- **tester.tap()** - Simulate tap
- **tester.pump()** - Rebuild widget

### Example Test Cases:
```dart
// Test if widget exists
expect(find.text('Hello'), findsOneWidget);

// Test if widget doesn't exist
expect(find.text('Goodbye'), findsNothing);

// Test button click
await tester.tap(find.byType(ElevatedButton));
await tester.pump();

// Enter text in TextField
await tester.enterText(find.byType(TextField), 'Test input');
```

---

## 18. DEPLOYMENT

### Android Application

**Steps to deploy Android app:**

**1. Create keystore:**
```bash
keytool -genkey -v -keystore my-key.jks -keyalg RSA -keysize 2048 -validity 10000 -alias my-alias
```

**2. Configure** `android/key.properties`:
```
storePassword=<password>
keyPassword=<password>
keyAlias=my-alias
storeFile=my-key.jks
```

**3. Update** `android/app/build.gradle`:
```gradle
signingConfigs {
    release {
        keyAlias keystoreProperties['keyAlias']
        keyPassword keystoreProperties['keyPassword']
        storeFile file(keystoreProperties['storeFile'])
        storePassword keystoreProperties['storePassword']
    }
}
```

**4. Build APK:**
```bash
flutter build apk --release
```

**5. Build App Bundle (for Play Store):**
```bash
flutter build appbundle --release
```

**6. Upload to Google Play Store**

### iOS Application

**Steps to deploy iOS app:**

**1. Open Xcode:**
```bash
open ios/Runner.xcworkspace
```

**2. Configure signing:**
- Select your team
- Choose bundle identifier

**3. Build for release:**
```bash
flutter build ios --release
```

**4. Create Archive in Xcode:**
- Product → Archive

**5. Upload to App Store Connect**

**6. Submit for Review**

---

## 19. DEVELOPMENT TOOLS

### Important Development Tools:

#### 1. Widget Sets
**Material Design** (Android style):
```dart
MaterialApp(...)
```

**Cupertino** (iOS style):
```dart
CupertinoApp(...)
```

#### 2. Visual Studio Code
- Lightweight editor
- Flutter extension available
- Good for small to medium projects

**Install Flutter extension:**
- Press Ctrl+Shift+X
- Search "Flutter"
- Click Install

**Useful shortcuts:**
- `Ctrl + Space` - Auto complete
- `F5` - Run app
- `Shift + F5` - Stop app
- `Ctrl + .` - Quick fix

#### 3. Dart DevTools
Browser-based tool for debugging

**Features:**
- **Inspector** - View widget tree
- **Timeline** - Performance analysis
- **Memory** - Check memory usage
- **Network** - Monitor API calls
- **Logging** - View console logs

**Open DevTools:**
```bash
flutter pub global activate devtools
flutter pub global run devtools
```

Or press **DevTools** button in VS Code debug toolbar

#### 4. Flutter SDK
Core toolkit for Flutter development

**Important commands:**
```bash
flutter doctor          # Check setup
flutter create myapp    # Create new app
flutter run             # Run app
flutter build           # Build app
flutter clean           # Clean build files
flutter upgrade         # Update Flutter
flutter pub get         # Get dependencies
flutter pub upgrade     # Update packages
flutter analyze         # Check code issues
flutter test            # Run tests
```

#### 5. Android Studio
- Full IDE
- Built-in emulator
- Good for large projects

#### 6. Hot Reload & Hot Restart
- **Hot Reload** (r) - Update UI instantly (keeps state)
- **Hot Restart** (R) - Restart app (loses state)

---

## 20. ADVANCED APPLICATIONS

### Common Advanced Features:

#### 1. Firebase Integration
- Authentication (Login/Signup)
- Cloud database
- Push notifications
- Analytics

#### 2. State Management (Provider)
```dart
// 1. Create provider
class Counter with ChangeNotifier {
  int _count = 0;
  int get count => _count;
  
  void increment() {
    _count++;
    notifyListeners();
  }
}

// 2. Provide to app
ChangeNotifierProvider(
  create: (context) => Counter(),
  child: MyApp(),
)

// 3. Use in widget
Consumer<Counter>(
  builder: (context, counter, child) {
    return Text('${counter.count}');
  },
)
```

#### 3. Camera & Image Picker
```dart
import 'package:image_picker/image_picker.dart';

final ImagePicker _picker = ImagePicker();
XFile? image = await _picker.pickImage(source: ImageSource.camera);
```

#### 4. Maps Integration
```dart
import 'package:google_maps_flutter/google_maps_flutter.dart';

GoogleMap(
  initialCameraPosition: CameraPosition(
    target: LatLng(28.6139, 77.2090),
    zoom: 14,
  ),
)
```

#### 5. Local Notifications
```dart
import 'package:flutter_local_notifications/flutter_local_notifications.dart';

FlutterLocalNotificationsPlugin flutterLocalNotificationsPlugin = 
    FlutterLocalNotificationsPlugin();

flutterLocalNotificationsPlugin.show(
  0,
  'Title',
  'Body',
  NotificationDetails(...),
);
```

#### 6. Shared Preferences (Save Data)
```dart
import 'package:shared_preferences/shared_preferences.dart';

// Save
SharedPreferences prefs = await SharedPreferences.getInstance();
await prefs.setString('username', 'John');

// Read
String username = prefs.getString('username') ?? '';
```

#### 7. Forms & Validation
```dart
final _formKey = GlobalKey<FormState>();

Form(
  key: _formKey,
  child: Column(
    children: [
      TextFormField(
        validator: (value) {
          if (value == null || value.isEmpty) {
            return 'Please enter text';
          }
          return null;
        },
      ),
      ElevatedButton(
        onPressed: () {
          if (_formKey.currentState!.validate()) {
            // Valid
          }
        },
        child: Text('Submit'),
      ),
    ],
  ),
)
```

#### 8. Themes (Dark/Light Mode)
```dart
MaterialApp(
  theme: ThemeData.light(),
  darkTheme: ThemeData.dark(),
  themeMode: ThemeMode.system, // or .light or .dark
)
```

---

## 21. IMPORTANT POINTS TO REMEMBER FOR EXAM

### Quick Revision Checklist:

✅ **Flutter Basics**
- Flutter is cross-platform framework by Google
- Uses Dart language
- Everything is a widget
- Hot reload for fast development

✅ **Widgets**
- StatelessWidget - Cannot change
- StatefulWidget - Can change
- Common widgets: Text, Container, Row, Column, ListView

✅ **State Management**
- setState() for local state
- Provider/scoped_model for global state
- State = data that can change

✅ **Navigation**
- Navigator.push() - Go to new screen
- Navigator.pop() - Go back
- Named routes for organized navigation

✅ **Layouts**
- Row - Horizontal
- Column - Vertical
- Stack - Overlap
- Container - Box with properties

✅ **Gestures**
- GestureDetector for handling taps, swipes
- onTap, onDoubleTap, onLongPress

✅ **API & Database**
- http package for REST API
- SQLite for local database
- Firestore for cloud database
- GET, POST, PUT, DELETE methods

✅ **Testing**
- Widget testing most common
- Use flutter_test package
- expect(), find, tester

✅ **Deployment**
- Android: Build APK or App Bundle
- iOS: Archive and upload to App Store
- Need signing/certificates

✅ **Packages**
- pub.dev for finding packages
- Add in pubspec.yaml
- flutter pub get to install

---

## SAMPLE QUESTIONS & ANSWERS

### Q1: What is Flutter?
**A:** Flutter is a free, open-source mobile application development framework created by Google. It allows developers to create cross-platform apps for Android, iOS, web, and desktop using a single codebase written in Dart language.

### Q2: Difference between StatelessWidget and StatefulWidget?
**A:** 
- **StatelessWidget**: Cannot change once created. Used for static content.
- **StatefulWidget**: Can change over time. Used for dynamic content that needs to update based on user interaction or data changes.

### Q3: What is setState()?
**A:** setState() is a method used in StatefulWidget to notify Flutter that the state has changed and the UI needs to be rebuilt.

### Q4: Explain Hot Reload.
**A:** Hot Reload is a feature that allows developers to see changes instantly without restarting the app. It preserves the app's state and updates only the changed code.

### Q5: What are the main layout widgets?
**A:** Row (horizontal), Column (vertical), Stack (overlap), Container (box), ListView (scrollable list), GridView (grid).

### Q6: How to navigate between screens?
**A:** Use Navigator.push() to go to a new screen and Navigator.pop() to go back.

### Q7: What is pubspec.yaml?
**A:** It's a configuration file that contains app metadata, dependencies (packages), assets, and other configurations.

### Q8: Explain async and await.
**A:** 
- **async**: Marks a function as asynchronous
- **await**: Waits for an asynchronous operation to complete
- Used for operations like API calls, file reading

### Q9: What is a Package in Flutter?
**A:** A package is reusable code library that adds functionality to your app. Types: Dart packages (pure Dart) and Plugin packages (contains native code).

### Q10: How to handle API calls in Flutter?
**A:** Use the http package with async/await:
```dart
final response = await http.get(Uri.parse('url'));
```

---

## IMPORTANT COMMANDS TO REMEMBER

```bash
# Check Flutter installation
flutter doctor

# Create new project
flutter create my_app

# Run app
flutter run

# Build APK
flutter build apk

# Get packages
flutter pub get

# Update packages
flutter pub upgrade

# Clean project
flutter clean

# Check for issues
flutter analyze

# Run tests
flutter test

# Check Flutter version
flutter --version

# Upgrade Flutter
flutter upgrade
```

---

## LAST MINUTE TIPS

1. **Understand Widgets** - Everything in Flutter is a widget
2. **Practice State Management** - Know when to use StatelessWidget vs StatefulWidget
3. **Remember Navigation** - Navigator.push() and Navigator.pop()
4. **Know Layout Widgets** - Row, Column, Stack, Container
5. **API Basics** - GET, POST requests using http package
6. **Testing Basics** - Widget testing with expect() and find
7. **Deployment Steps** - Know how to build APK for Android
8. **Common Packages** - http, provider, sqflite, shared_preferences
9. **Dart Basics** - Variables, functions, classes, async/await
10. **Architecture** - Understand widget tree and state management

---

## ALL THE BEST! 🎯

**Remember:**
- Flutter is easy once you understand widgets
- Practice makes perfect
- Everything is a widget
- State management is key
- Don't panic, take your time

**Study Strategy:**
- Day 1: Basics, Widgets, Layouts
- Day 2: State Management, Navigation, Gestures
- Day 3: API, Database, Testing, Deployment
- Day 4: Quick revision and practice questions

---

**Good luck with your exam on November 2, 2025! You've got this! 💪**
