# Cricket Shot Detection

Clean project repository for the `EE655` cricket shot detection course project.

This repo contains the Streamlit app, inference code, the final reference notebook, and the model/result assets required to run the project.

## Kept Files

- `app.py` - Streamlit UI for single-video prediction and video comparison
- `cricket_notebook_model.py` - model loading, frame sampling, inference, and PDF report generation
- `fork-of-cricket-shot-detection (3).ipynb` - final reference notebook
- `results_current/` - checkpoints and result plots/CSV files used by the app
- `.streamlit/config.toml` - Streamlit configuration
- `requirements.txt` - Python dependencies

## Shot Classes

- `cover`
- `defense`
- `flick`
- `hook`
- `late_cut`
- `lofted`
- `pull`
- `square_cut`
- `straight`
- `sweep`

## Run Locally

```powershell
python -m venv .venv
.\.venv\Scripts\activate
pip install -r requirements.txt
streamlit run app.py
```

## Notes

- `results_current/` is included because the app depends on the trained checkpoints and summary assets.
- `fork-of-cricket-shot-detection (3).ipynb` is the retained notebook reference for the final project pipeline.
