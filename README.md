# 🐳 CI/CD Pipeline - Telco Churn Model

Repository ini merupakan kelanjutan dari tahapan *preprocessing* pada kelas **Membangun Sistem Machine Learning**, berfokus pada implementasi **Continuous Integration & Continuous Deployment (CI/CD)** untuk model Machine Learning menggunakan **Docker** dan **GitHub Actions**.

## 📌 Deskripsi Proyek
Proyek ini mengemas model prediksi Telco Customer Churn (menggunakan *RandomForestClassifier*) ke dalam sebuah *Docker Image* yang terisolasi. Setiap kali ada perubahan kode pada repository ini, GitHub Actions akan secara otomatis:
1. Melakukan *Checkout* kode.
2. *Login* ke sistem Docker Hub.
3. Melakukan *Build* Docker Image berdasarkan `Dockerfile` yang telah dikonfigurasi.
4. Mendorong (*Push*) Image tersebut ke *registry* publik Docker Hub.

Selain itu, proyek ini juga mengimplementasikan pelacakan eksperimen (*experiment tracking*) yang terintegrasi dengan **DagsHub**.

## ⚙️ Teknologi yang Digunakan
* **Python 3.12** & **Scikit-Learn**
* **MLflow** (Experiment Tracking)
* **Docker** (Containerization)
* **GitHub Actions** (CI/CD Pipeline)

## 🚀 Docker Hub URL
Image hasil *build* CI/CD dari repository ini dapat ditarik (*pull*) secara publik melalui Docker Hub pada tautan berikut:
`https://hub.docker.com/repository/docker/mysteryworld3/mlops-telco-model/general`
