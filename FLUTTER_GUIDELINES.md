# Flutter Development Guidelines

## 🎯 Code Standards

### File Structure
```
lib/
├── core/
│   ├── constants/
│   ├── errors/
│   ├── usecases/
│   └── utils/
├── features/
│   └── [feature_name]/
│       ├── data/
│       ├── domain/
│       └── presentation/
└── main.dart
```

### Naming Conventions
- **Files & Folders**: snake_case
- **Classes**: PascalCase
- **Variables & Functions**: camelCase
- **Constants**: SCREAMING_SNAKE_CASE

### Code Quality
- ✅ Follow Dart Style Guide
- ✅ Use effective Dart patterns
- ✅ Write meaningful comments
- ✅ Implement proper error handling
- ✅ Maintain test coverage > 80%

## 🏗️ Architecture Patterns

### Clean Architecture
- **Presentation Layer**: UI, Widgets, BLoCs
- **Domain Layer**: Entities, Use Cases, Repository Interfaces
- **Data Layer**: Repository Implementation, Data Sources, Models

### State Management
- **BLoC**: For complex state management
- **Provider**: For simple dependency injection
- **Riverpod**: For advanced reactive programming

## 🧪 Testing Strategy

### Test Pyramid
1. **Unit Tests** (70%): Business logic validation
2. **Widget Tests** (20%): UI component testing
3. **Integration Tests** (10%): End-to-end scenarios

### Best Practices
- Write tests before implementation (TDD)
- Mock external dependencies
- Test edge cases and error scenarios
- Use descriptive test names

## 🚀 Performance Optimization

### Key Principles
- Use `const` constructors when possible
- Implement proper widget lifecycle management
- Optimize list rendering with `ListView.builder`
- Minimize widget rebuilds
- Use `RepaintBoundary` for expensive widgets

### Memory Management
- Dispose of controllers and streams
- Avoid memory leaks in listeners
- Use `AutomaticKeepAliveClientMixin` wisely
- Profile app performance regularly

## 📱 UI/UX Guidelines

### Design Principles
- Follow platform conventions (Material/Cupertino)
- Ensure accessibility compliance
- Implement responsive design
- Use consistent spacing and typography
- Provide meaningful feedback to users

### Animation Guidelines
- Use `AnimationController` for custom animations
- Implement `Hero` animations for navigation
- Keep animations under 300ms for UI interactions
- Use `Curve` classes for natural motion

## 🔧 Development Tools

### Essential Extensions
- Flutter/Dart extensions for VS Code
- Flutter Inspector for debugging
- Flutter Performance for optimization
- Dart Code Metrics for code quality

### Useful Packages
- **State Management**: flutter_bloc, provider, riverpod
- **Networking**: dio, http
- **Local Storage**: shared_preferences, hive
- **Navigation**: go_router, auto_route
- **UI**: flutter_screenutil, cached_network_image
- **Testing**: mockito, bloc_test

---

*These guidelines ensure consistent, maintainable, and high-quality Flutter applications.*
