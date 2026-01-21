# 📝 data_ml — Creating requirements.txt / Erstellung von requirements.txt

Instruction for creating a `requirements.txt` file from the `data_ml` environment in Anaconda (Windows).
Anleitung zum Erstellen einer `requirements.txt`-Datei aus der Umgebung `data_ml` in Anaconda (Windows).

---

## 1️⃣ Open Anaconda Prompt / Anaconda Prompt öffnen

Make sure you see the base environment, for example:

```
(base) C:\Users\...
```

Stelle sicher, dass die Basisumgebung sichtbar ist, z. B.:

```
(base) C:\Users\...
```

---

## 2️⃣ Activate `data_ml` environment / Aktivieren der Umgebung `data_ml`

```bash
conda activate data_ml
```

After this, the prompt should look like:

```
(data_ml) C:\Users\...
```

Dies bedeutet, dass alle Befehle in der richtigen Umgebung ausgeführt werden.

---

## 3️⃣ Navigate to your project folder (optional) / Wechsle in den Projektordner (optional)

It is recommended to create `requirements.txt` directly in the project folder so it can be used for GitHub or shared with colleagues.

```bash
cd C:\Users\UserS2025\Projects\data_ml_project
```

Check the current directory:

```bash
cd
```

or

```bash
dir
```

Überprüfe das aktuelle Verzeichnis:

```bash
cd
```

oder

```bash
dir
```

---

## 4️⃣ Create the requirements.txt file / Erstellen der requirements.txt Datei

```bash
pip freeze > requirements.txt
```

What happens / Was passiert:

* `pip freeze` — outputs all installed packages with exact versions / gibt alle installierten Pakete mit exakten Versionen aus
* `> requirements.txt` — writes this list to `requirements.txt` / schreibt diese Liste in `requirements.txt`

The file will appear in the **current project folder** / Die Datei wird im **aktuellen Projektordner** erstellt.

---

## 5️⃣ Check the file / Datei prüfen

```bash
dir requirements.txt
```

Open the file with Notepad or any editor. It should look like:

```
numpy==1.25.2
pandas==2.1.0
matplotlib==3.8.0
seaborn==0.13.2
scikit-learn==1.3.0
scipy==1.12.0
jupyter==1.0.0
ipykernel==6.27.0
```

Öffne die Datei mit Notepad oder einem Editor. Sie sollte etwa so aussehen:

```
numpy==1.25.2
pandas==2.1.0
matplotlib==3.8.0
seaborn==0.13.2
scikit-learn==1.3.0
scipy==1.12.0
jupyter==1.0.0
ipykernel==6.27.0
```

---

## 6️⃣ Using requirements.txt on another computer / Verwendung von requirements.txt auf einem anderen Rechner

To recreate the same environment on another machine:

```bash
pip install -r requirements.txt
```

✅ All packages will be installed with the same versions as in your `data_ml` environment / Alle Pakete werden mit denselben Versionen wie in deiner `data_ml` Umgebung installiert.

---

## 💡 Tip / Tipp

* Run `pip freeze > requirements.txt` after installing all needed libraries and before uploading the project to GitHub / Führe `pip freeze > requirements.txt` aus, nachdem alle benötigten Bibliotheken installiert wurden und bevor du das Projekt auf GitHub hochlädst.
* If you add new libraries, **update** the requirements.txt with the same command / Wenn du neue Bibliotheken hinzufügst, **aktualisiere** die requirements.txt mit demselben Befehl.

---

📌 Save this file as `data_ml_Requirements_Instructions.md` and keep it in the root of your project / Speichere diese Datei als `data_ml_Requirements_Instructions.md` und lege sie in das Stammverzeichnis des Projekts.

