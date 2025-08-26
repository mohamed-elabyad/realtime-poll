# Laravel Livewire Poll App

A simple **polling application** built with the latest versions of **Laravel** and **Livewire**.  
This project was mainly created to practice and get familiar with Livewire concepts.

---

## Features
- **Livewire Components**  
  - **PollForm**:  
    - Input field for poll question  
    - Add & remove options dynamically  
    - Validation with real-time error messages  
    - Dispatches a `pollCreated` event after saving  

  - **PollList**:  
    - Listens for `pollCreated` and re-renders automatically  
    - Fetches all polls from the database  
    - Displays them on the same page without refresh  
    - Includes a **vote** button to increment vote count instantly  

- **Validation**: Server-side validation handled by Livewire.  
- **Realtime Updates**: All interactions happen without page reloads or manual AJAX requests.  
- **Latest Stack**: Built using **Laravel 12** and **Livewire 3**.

---

## Installation
1. Clone the repository:
   bash:
   git clone https://github.com/yourusername/livewire-poll-app.git
   cd livewire-poll-app

---

## Install dependencies:

composer install
npm install && npm run dev

### Set up your .env file and run migrations:
cp .env.example .env
php artisan key:generate
php artisan migrate

### Serve the application:
php artisan serve

---

## Usage
Create a new poll by entering a question and adding/removing options.

Submit the form → poll is saved and event pollCreated is dispatched.

Poll list re-renders automatically and shows the new poll.

Click the vote button to increase the vote count in real-time.

---

## Tech Stack
Laravel 12

Livewire 3

Tailwind CSS (for styling)

---

## Notes
This is a practice project to explore how Livewire works with events, validation, and real-time UI updates.
Everything runs smoothly on a single page, without full page reloads.

---

## Made with Love ❤️ by Mohamed Elabyad
If you have any questions or want to get in touch, feel free to reach out: 📧 Email: m.elabyad.work@gmail.com
