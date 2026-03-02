# 🔐 CertVerify – Blockchain-Based Certificate Verification System

CertVerify is a secure and tamper-proof certificate issuing and verification platform that leverages **Blockchain technology** and **SHA-256 hashing** to prevent academic fraud and certificate forgery.

It ensures that issued certificates cannot be altered, duplicated, or manipulated.

---

## 🛠️ Tech Stack

- 🐍 Python (FastAPI Backend)
- ⛓️ Ethereum Blockchain (Web3.py)
- 🔐 SHA-256 File Hashing
- 🌐 REST APIs
- 🗄️ JSON-based User Storage
- 🧪 Debug & Testing Utilities

---

## 🚀 Key Features

✅ Issue certificates with blockchain hash registration  
✅ Verify certificates via file upload  
✅ SHA-256 hash-based integrity validation  
✅ Smart contract-based immutability  
✅ Admin statistics & certificate explorer APIs  
✅ Student ID-based verification  
✅ Debug and validation scripts for testing  

---

## 🏗️ Project Structure

```
CertVerify/
│
├── backend/                      # FastAPI backend application
├── frontend/                     # Frontend UI
├── ml/                           # Machine learning components (if applicable)
├── models/                       # Saved ML models
├── uploads/                      # Uploaded certificate files
│
├── backend_test.py               # Backend API testing
├── check_blockchain_direct.py    # Direct blockchain verification
├── check_user_file_hash.py       # SHA-256 hash comparison
├── debug_store.py                # Debug blockchain storage
├── debug_verify.py               # Debug certificate verification
├── issue_real_cert.py            # Issue sample certificate
├── issue_user_file.py            # Issue uploaded certificate
├── verify_issue.py               # Verify issue status
├── verify_student_id.py          # Student ID verification
│
├── users.json                    # User database (JSON)
├── real_cert.png                 # Sample certificate
└── README.md                     # Documentation
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/yourusername/CertVerify.git
cd CertVerify
```

---

### 2️⃣ Create Virtual Environment (Recommended)

```bash
python -m venv venv
venv\Scripts\activate   # Windows
```

For Mac/Linux:
```bash
source venv/bin/activate
```

---

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

If `requirements.txt` is not available:

```bash
pip install fastapi uvicorn web3 requests python-multipart
```

---

### 4️⃣ Start Backend Server

```bash
uvicorn main:app --reload
```

Backend runs at:

```
http://localhost:8000
```

Swagger API Docs:

```
http://localhost:8000/docs
```

---

## ⛓️ Blockchain Setup

Run a local Ethereum blockchain using:

- Hardhat  
or  
- Ganache  

Default RPC URL:

```
http://127.0.0.1:8545
```

Smart contract interactions are handled via Web3.py.

---

## 🔍 How Certificate Verification Works

1. Certificate file is uploaded.
2. System generates SHA-256 hash of the file.
3. Hash is stored on the Ethereum blockchain.
4. During verification:
   - Uploaded file is re-hashed.
   - Compared against stored blockchain hash.
   - System returns: ✅ Valid or ❌ Fake.

---

## 🧪 Testing & Debug Scripts

Run backend test:

```bash
python backend_test.py
```

Debug blockchain storage:

```bash
python debug_store.py
```

Verify certificate upload:

```bash
python debug_verify.py
```

Direct blockchain verification:

```bash
python check_blockchain_direct.py
```

---

## 📊 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | /api/issue | Issue certificate |
| POST | /api/upload | Verify certificate |
| GET | /api/explorer | View issued certificates |
| GET | /api/admin/stats | View admin statistics |
| POST | /auth/register | Register user |
| POST | /auth/login | User login |

---

## 🔐 Security Features

- SHA-256 cryptographic hashing
- Blockchain immutability
- Secure REST APIs
- Student ID validation
- Certificate integrity verification
- Tamper detection mechanism

---

## 🎯 Use Cases

- Universities & Colleges
- Online Certification Platforms
- Skill Training Institutes
- Government Credential Systems
- Digital Badge Verification Platforms

---

## ⭐ Future Enhancements

- Deploy smart contract on Ethereum Testnet (Sepolia/Goerli)
- IPFS integration for decentralized storage
- QR Code-based certificate validation
- Enhanced frontend dashboard
- AI-based forged certificate detection

---

## 👩‍💻 Author

**Sai Dinesh Somavarapu**  
Blockchain & Backend Developer  
2025
