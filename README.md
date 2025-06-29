# Campus Library Info Chatbot

This is a functional, no-code chatbot built using **Dialogflow ES** and deployed via **Dialogflow Messenger**, designed to simulate a university library assistant. It demonstrates core product skills relevant to LimeChat's Associate Product Manager role, including conversation design, user flow mapping, and fulfillment logic.

---

## Features

* **Multi-intent handling**
  Responds to user queries around:

  * Library timings
  * Book availability
  * Study room reservations (with slot-filling)

* **Webhook fulfillment**
  Implements Dialogflow’s Inline Editor (Node.js + Firebase Functions) to:

  * Check book availability from a mock catalog
  * Confirm room bookings with structured parameters

* **Slot-filling and system entities**
  Utilizes `@sys.date`, `@sys.time`, and `@sys.duration` to guide users through multi-turn booking flows.

* **Deployed via Dialogflow Messenger**
  Fully testable in-browser chatbot, with no external API costs or setup.

---

## Live Demo

**Try it here:**
[Campus Library Bot Web Demo](https://kshitij-ekantikashya.github.io/Campus-Lib-Bot/)

---

## Tech Stack

| Tool               | Use Case                              |
| ------------------ | ------------------------------------- |
| Dialogflow ES      | Natural language understanding        |
| Inline Editor      | Webhook logic (Node.js fulfillment)   |
| Firebase Functions | Serverless backend environment        |
| GitHub Pages       | Hosting the embedded chatbot frontend |

---

## Example Conversations

### Book Lookup

```
User: Do you have The Hobbit?
Bot: Yes, "The Hobbit" is available.
```

### Slot Reservation

```
User: I want to reserve a study slot
Bot: Which date would you like to book?
User: Tomorrow
Bot: What time?
User: 3 PM
Bot: For how long?
User: 1 hour
Bot: Your study slot has been reserved for Sun Jun 30 2025 at 15:00 for 1 hour.
```

---

## Repository Contents

```
campus-library-bot/
├── index.html       # Web UI embedding Dialogflow Messenger
├── README.md        # Project overview
└── screenshots/     # Optional: Dialogflow interface screenshots
```

---

## Author

**Kshitij Ranjan**
Product Management
[LinkedIn](https://linkedin.com/in/kshitij-ranjan21)

---

## Notes

* Designed as a skills demonstration project.
* No paid APIs, keys, or third-party integrations were used.
* Easily extendable to WhatsApp and other messaging platforms.
