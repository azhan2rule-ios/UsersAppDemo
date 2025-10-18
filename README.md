# UsersApp

A simple SwiftUI application that fetches and displays a list of users from a remote API. Tapping on a user navigates to a detail view.

## Features

- MVVM architecture with clean separation of concerns.
- Async networking using `URLSession` and Swift Concurrency (`async/await`).
- Custom protocol-based `NetworkHandler` and `DecoderHandler` for better testability.
- Uses `NavigationStack` for modern navigation in SwiftUI.
- Error handling and UI feedback.

## Project Structure

- **Network.swift**: Handles API calls and JSON decoding using protocols (`NetworkHandler`, `DecoderHandler`).
- **User.swift**: Defines the `Users` model conforming to `Codable`.
- **UserListView.swift**: Displays a list of users using `List` and navigates to detail view.
- **UserDetailView.swift**: Shows detailed user information.
- **UserVM.swift**: ViewModel handling data fetching and state management using `@Published`.
- **UserRepo.swift**: Repository layer responsible for coordinating network and decoding logic.

## API

- **Base URL**: `https://fake-json-api.mock.beeceptor.com/`
- **Endpoint**: `/users` – Returns a list of users.

## Getting Started

1. Clone the repository.
2. Open `UsersApp.xcodeproj` in Xcode.
3. Build and run on simulator or device.

## Requirements

- iOS 15.0+
- Xcode 13+
- Swift 5.5+

## Author

Azhaan Hasib

