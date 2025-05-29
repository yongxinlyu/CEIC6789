# 📘 Contributing to the Course Jupyter Book

Thank you for helping improve this course! This guide explains how to add or update content in the Jupyter Book.

---

## 📁 Project Structure

The repository is organized as follows:

- `Info/` — Course info pages (overview, learning objectives, resources)
- `Lectures/lecture_X/` — Lecture materials grouped by lecture number
- `Tutorials/tutorial_X/` — Tutorials grouped by tutorial number

---

## ➕ How to Add a New Lecture or Tutorial

1. **Create a new folder** in the appropriate directory:
   - Example: `Lectures/lecture_3/` or `Tutorials/tutorial_2/`

2. **Add an info Markdown file**:
   - Name it like `Lecture3_info.md` or `tutorial2_info.md`
   - Include a short description, and links to the PDF slides and video (if available)

3. **Add your notebooks**:
   - Place relevant `.ipynb` files in the same folder
   - Add slide PDFs (`.pdf`) or video embed `.md` files as needed

4. **Update `_toc.yml`**:
   - Reference each file using relative paths **without extensions** (`.md` or `.ipynb`)
   - Use `sections:` to group notebooks under the main info file

   ### Example entry in `_toc.yml`:

   ```yaml
   - file: Lectures/lecture_3/Lecture3_info
     sections:
       - file: Lectures/lecture_3/Lecture3_notebook