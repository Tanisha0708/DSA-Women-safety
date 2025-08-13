# 🛡️ WomenSafety - A Secure Platform

**WomenSafety** is a **Java-based console application** focused on empowering women by providing a **secure and supportive virtual environment**.  
The platform allows users to:
- **Ask queries related to laws & regulations**
- **Draft formal complaints**
- **Interact with an AI-powered virtual assistant**
- **Get assistance in unsafe situations**

This project was developed with the vision of creating a **quick, reliable, and user-friendly** tool that can help women in need, even in **critical moments**.

---

## 🚀 Features
- 📜 **Law & Regulation Queries** – Get instant responses to questions about women's rights and safety laws.
- 📝 **Formal Complaint Drafting** – Create complaint templates to file with authorities.
- 🤖 **AI-powered Virtual Assistant** – Offers emotional and procedural guidance in unsafe situations.
- 🔒 **Secure & Reliable** – Built with **Java** and **DSA** concepts for speed and efficiency.
- 🎨 **Attractive Console UI** – Clean, easy-to-use, and visually appealing interface.

---

## 🛠️ Tech Stack
- **Language:** Java
- **Concepts Used:** Data Structures & Algorithms (Java)
- **Other Tools:** Java I/O, String Handling, OOP Principles

---

## Code Output 
# Create a consolidated sample output transcript and a sample complaint draft file
from datetime import datetime

banner = """\
╔═══════════════════════════════════════════════════════╗
║         W O M E N S A F E T Y   C H A T B O T         ║
║     Your console ally for awareness and assistance     ║
╚═══════════════════════════════════════════════════════╝
"""

menu = """\
◆ Home
1. Ask about laws & rights   (Trie + KMP powered)
2. Draft a formal complaint  (saves to .txt)
3. Safety assistant          (guided steps + SOS)
4. Resources & safety tips
5. Manage emergency contacts (PriorityQueue)
6. View session history      (Stack)
7. Exit
"""

law_flow = """\
────────────────────────────────────────────────────────────
◆ Ask about Laws & Rights (general awareness)
Tip: Type :suggest cyber  → Suggestions: cyber, cyberharassment
Q> what to do in case of cyber harassment in instagram?

A> Cyber harassment includes online threats, doxxing, non-consensual image sharing, and abuse. Collect screenshots/URLs, use platform reporting tools, and change passwords.
Next steps: document evidence, ensure personal safety, and consider contacting trusted people or helplines (112 / 181).
"""

complaint_preview = """\
────────────────────────────────────────────────────────────
◆ Complaint Desk (Draft a Formal Complaint)

Preview
To,
Station House Officer, Shivajinagar Police Station, Pune

Date: 13 Aug 2025

Subject: Complaint regarding online harassment

Respected Sir/Madam,

I, Tanisha Chavan (Phone: 9000000000, Email: tanisha@example.com), residing at Pune, Maharashtra,
wish to formally lodge a complaint regarding the incident that occurred on 12 Aug 2025 at Pune City.

Details of the incident:
I have been repeatedly harassed on Instagram via abusive DMs and threats. I have collected screenshots of messages and profile URLs.

Accused involved (if known): @user123 (Instagram handle)

Attachments enclosed: screenshots.zip

I request that appropriate legal action be taken as per the applicable laws. I am willing to cooperate and provide any further information required.

Thank you.

Sincerely,
Tanisha Chavan
Pune, Maharashtra
Phone: 9000000000 | Email: tanisha@example.com
Saved: Complaint_Tanisha_Chavan_20250813_190500.txt
"""

safety_flow_ok = """\
────────────────────────────────────────────────────────────
◆ Safety Assistant

Are you currently in immediate danger? (yes/no): no
Are you in a safe location right now? (yes/no): no
⚠ If possible, move to a safer, well-lit public area. Keep your phone ready.
Do you want a quick personal safety plan checklist? (yes/no): yes
• Share your trip with a trusted contact and turn on location sharing.
• Keep your phone charged; carry a portable power bank if possible.
• Identify safe spots nearby (police station, hospital, busy stores).
• If threatened, be loud and attract attention; move towards crowds.
• Trust your instincts; choose safer routes even if longer.
• Keep emergency numbers handy: 112 (India), 181 (Women Helpline).
• Preserve evidence: messages, photos, medical records if any.
• After the incident, consider seeking professional support.
Generate an SOS message template you can copy? (yes/no): yes

┌──────────────────────────────────────────────────────────────┐
│ SOS! I need urgent help.                                     │
│ My live location: <share current location link>              │
│ Details (brief): <what happened>                             │
│ Call me ASAP: <your phone>                                   │
│ Nearest landmark: <landmark>                                 │
│ If unreachable, contact: Women Helpline (181)                │
│ Time: 13 Aug 2025, 19:05                                     │
└──────────────────────────────────────────────────────────────┘
Top emergency contacts (by priority):
  - Local Helpline (112) [priority 10]
  - Women Helpline (181) [priority 9]
  - Trusted Friend (9999999999) [priority 5]
  - Parent (8888888888) [priority 4]
Note: This app cannot send messages. Copy the SOS text above and share via your phone.
"""

safety_flow_danger = """\
────────────────────────────────────────────────────────────
◆ Safety Assistant

Are you currently in immediate danger? (yes/no): yes
⚠ If safe, consider calling emergency number: 112 (India) or your local emergency number.
Preparing quick SOS info ▮▮▮▮▮▮▮▮▮▮▮▮▮▮▮ done

┌──────────────────────────────────────────────────────────────┐
│ SOS! I need urgent help.                                     │
│ My live location: <share current location link>              │
│ Details (brief): <what happened>                             │
│ Call me ASAP: <your phone>                                   │
│ Nearest landmark: <landmark>                                 │
│ If unreachable, contact: Local Helpline (112)                │
│ Time: 13 Aug 2025, 19:06                                     │
└──────────────────────────────────────────────────────────────┘
"""

contacts_flow = """\
────────────────────────────────────────────────────────────
◆ Manage Emergency Contacts (PriorityQueue)

1. View contacts
2. Add contact
3. Remove top-priority contact
4. Clear all
5. Back

Before:
1. Local Helpline (112) [priority 10]
2. Women Helpline (181) [priority 9]
3. Trusted Friend (9999999999) [priority 5]
4. Parent (8888888888) [priority 4]

Add contact → Name: Roommate, Phone: 7777777777, Priority: 8
✔ Contact added.

After:
1. Local Helpline (112) [priority 10]
2. Women Helpline (181) [priority 9]
3. Roommate (7777777777) [priority 8]
4. Trusted Friend (9999999999) [priority 5]
5. Parent (8888888888) [priority 4]

Remove top-priority → Removed: Local Helpline (112) [priority 10]
"""

history_resources = """\
────────────────────────────────────────────────────────────
◆ Session History (latest first)
• complaint:Complaint regarding online harassment
• lawQ:what to do in case of cyber harassment in instagram?
• menu:2
• menu:1
Undo last action? (y/n): y
ℹ Undone: complaint:Complaint regarding online harassment

────────────────────────────────────────────────────────────
◆ Resources & Tips
┌───────────────────────────────────────────────────────────┐
│ Emergency: 112 (India)                                    │
│ Women Helpline: 181                                       │
│ Cybercrime Portal: https://cybercrime.gov.in              │
│ Local Police: Nearest station or district website         │
│ Legal Aid: State/District Legal Services Authorities      │
└───────────────────────────────────────────────────────────┘
"""

closing = """\
────────────────────────────────────────────────────────────
✔ Goodbye. Stay safe and take care.
"""

full_transcript = "\n".join([banner, menu, law_flow, complaint_preview, safety_flow_ok, safety_flow_danger, contacts_flow, history_resources, closing])

# Write sample transcript file
transcript_path = "/mnt/data/womensafety_sample_output.txt"
with open(transcript_path, "w", encoding="utf-8") as f:
    f.write(full_transcript)

# Create a separate example complaint draft file
complaint_file_path = "/mnt/data/Complaint_Tanisha_Chavan_Example.txt"
complaint_content = complaint_preview.split("Preview\n",1)[1].split("Saved:",1)[0].rstrip() + "\n"
with open(complaint_file_path, "w", encoding="utf-8") as f:
    f.write(complaint_content)

transcript_path, complaint_file_path

