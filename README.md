# 🔥 LithoLab PRO — Lithophane Engine

LithoLab PRO generates **3D-printable lithophanes (STL)** and simulates **realistic light transmission** in the browser using GPU shaders.

---

## ⚙️ Setup (Fast + Minimal)

### 1. Backend (Python)

```bash
cd backend
pip install -r requirements.txt
uvicorn main:app --reload
```

Runs at:

```
http://localhost:8000
```

---

### 2. Frontend

Just open:

```
frontend/index.html
```

(Use Chrome / Edge)

---

## 🧪 Usage

1. Upload image
2. Generate STL
3. Load STL in viewer
4. Toggle lamp → see light effect

---

## 💡 Key Concept

Lithophanes are NOT normal 3D models.

Brightness depends on **thickness**, not surface lighting:

```
light = exp(-alpha * thickness)
```


## 🖨️ Print Settings

* 100% infill
* 0.1–0.12mm layer height
* White PLA
* Print vertically

---

## 🚀 Summary

* Backend → builds solid STL
* Frontend → simulates light through thickness
* Shader → approximates real plastic behavior

---

Built for **real lithophane results**, not fake previews.
