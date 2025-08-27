# Task 1: Create Your First Mobile App

## Objective
Set up your first mobile application using the Expo Router template, document the scaffolding process, and understand the file structure of a React Native application using Expo.

## Required Steps

### Step 1: Navigate to Your Project Directory
```bash
cd prodev-mobile-setup
```

### Step 2: Set Up Your Project
Initialize a new Expo project using the latest Expo Router template:
```bash
npx create-expo-app@latest .
```

### Step 3: Modify the Home Screen
1. Open `app/(tabs)/index.tsx`
2. Locate the default text **Welcome!**
3. Change it to **First App Created**

### Step 4: Run and Test Your Application
Start the Expo development server:
```bash
npx expo start
```

**Testing on Devices:**
- **iOS Devices**: Scan the QR code in the terminal using your phone's Camera app
- **Android Devices**: Scan the QR code using the Expo Go app

### Step 5: Reset the Application
Run the reset command and observe its effects:
```bash
npm run reset-project
```

## Documentation Requirements

### README.md Must Include:
- [ ] Steps you followed for scaffolding
- [ ] Observations from the `reset-project` command
- [ ] Setup process documentation
- [ ] Any challenges faced during development

## Repository Structure

```
prodev-mobile-setup/
├── prodev-mobile-app-0x00/
│   ├── README.md
│   ├── app-example/
│   │   ├── app/
│   │   │   └── (tabs)/
│   │   │       └── index.tsx
│   │   └── constants/
│   │       └── Colors.tsx
│   └── [other project files]
```

## Required Files to Submit:
- `README.md` - Documentation of your setup process
- `app-example/app/(tabs)/index.tsx` - Modified home screen
- `app-example/` - Complete app directory
- `app-example/constants/Colors.tsx` - Color constants file

## Sample README.md Template

```markdown
# First Mobile App - Setup Documentation

## Scaffolding Steps Followed

1. **Project Directory Setup**
   - Navigated to `prodev-mobile-setup` directory
   - Initialized Expo project with Router template

2. **Project Creation**
   - Command used: `npx create-expo-app@latest .`
   - Template: Expo Router (latest)

3. **Home Screen Modification**
   - File modified: `app/(tabs)/index.tsx`
   - Changed "Welcome!" to "First App Created"

4. **Testing Process**
   - Started development server with `npx expo start`
   - Tested on [iOS/Android] device using [Camera app/Expo Go]

## Reset Project Observations

After running `npm run reset-project`:
- [Document what happened]
- [List files that were affected]
- [Note any changes in project structure]
- [Mention if the modification was preserved or lost]

## Challenges Faced
## Reset Project Observations

After running `npm run reset-project` and choosing "Y":

### What Happened:
- Files moved to `/app-example` directory
- Fresh Expo template created in root
- My "First App Created" modification preserved in `app-example/app/(tabs)/index.tsx`

### Errors Encountered:
- Import errors in moved files: `Cannot find module '@/components/ThemedView'`
- ESLint errors: `Unable to resolve path to module '@/components/ThemedView'`

### Root Cause:
- Moved files still reference components from the original project structure
- The `/app-example` folder is isolated and missing the required dependencies
- This is expected behavior when files are moved without their full dependency tree

### Project Structure After Reset:
- Root: Fresh Expo template
- `/app-example`: Contains my modified files (with broken imports)
- My "First App Created" text is preserved in `app-example/app/(tabs)/index.tsx`

## Screenshots
- [Optional: Include screenshots of your app running]
```

## Important Notes

- Ensure Expo Go is installed on your physical device
- Make sure Node.js LTS is installed
- Document the reset command effects thoroughly
- Keep the modified text "First App Created" in your final submission

## Success Criteria

✅ Project successfully created with Expo Router template  
✅ Home screen text modified to "First App Created"  
✅ Application runs successfully on physical device  
✅ Reset command executed and documented  
✅ README.md contains all required documentation  
✅ All required files present in correct directory structure