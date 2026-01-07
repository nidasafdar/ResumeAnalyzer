# 🚀 Streamlit Cloud Deployment Guide

## Your Resume Analyzer is ready to deploy!

### Step 1: Push the new files to GitHub

The necessary configuration files have been created:
- ✅ `requirements.txt` (moved to root)
- ✅ `packages.txt` (system dependencies)
- ✅ `.streamlit/config.toml` (Streamlit configuration)
- ✅ `setup.sh` (spacy model download script)
- ✅ `App.py` (main application file in root)

### Step 2: Deploy to Streamlit Cloud

1. **Go to Streamlit Cloud**: https://streamlit.io/cloud
2. **Sign in** with your GitHub account
3. **Click "New app"**
4. **Select your repository**: `nidasafdar/ResumeAnalyzer`
5. **Main file path**: `App.py`
6. **Click "Deploy"**

### Step 3: Wait for Deployment

Streamlit Cloud will:
- Install all dependencies from `requirements.txt`
- Install system packages from `packages.txt`
- Run the setup script to download spacy models
- Deploy your app

### Step 4: Get Your Live URL

Once deployed, you'll get a URL like:
**`https://resumeanalyzer-[random-id].streamlit.app`**

You can customize this URL in the Streamlit Cloud settings!

---

## Alternative Deployment Options

### Option 2: Render.com (FREE)
1. Go to https://render.com
2. Create a new Web Service
3. Connect your GitHub repository
4. Build Command: `pip install -r requirements.txt && python -m spacy download en_core_web_sm`
5. Start Command: `streamlit run App.py --server.port=$PORT --server.address=0.0.0.0`

### Option 3: Hugging Face Spaces (FREE)
1. Go to https://huggingface.co/spaces
2. Create a new Space (select Streamlit)
3. Upload your files or connect GitHub
4. Auto-deploys!

---

## 🎉 Recommended: Streamlit Cloud
It's the easiest and specifically designed for Streamlit apps!
