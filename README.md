# Head Pose Estimation (MediaPipe + OpenCV)

This module estimates **3D head pose** from video using facial landmarks and OpenCV PnP.

It is part of a multimodal cheating detection system.

---

## 🧠 Method

- Detect face landmarks (MediaPipe)
- Map 2D points to 3D face model
- Apply `cv2.solvePnP`
- Extract head rotation (rvec) and translation (tvec)

---

## 📌 Key Landmarks

Nose, Chin, Eyes, Mouth corners

---

## ⚙️ Output

- Rotation vector (head direction)
- Translation vector (position)

---

## 🚀 Run

```bash
python head_pose.py
cap.release()
cv2.destroyAllWindows()
