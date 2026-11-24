# Third-party notices / Hinweise zu Komponenten Dritter

Quick Hubble Creator (QHC) uses the following open-source components. They remain under their own licenses; the texts are
available at the given links and in the packages themselves. /
QHC benutzt die folgenden Open-Source-Komponenten. Sie bleiben unter ihren eigenen Lizenzen; die Lizenztexte stehen unter den
Links und in den Paketen selbst.

| Component | Use in QHC | License | Link |
|---|---|---|---|
| Qt for Python (PySide6, Shiboken6) | user interface | LGPL v3 (Qt 6 modules used: QtCore, QtGui, QtWidgets) | https://doc.qt.io/qtforpython-6/ , https://www.gnu.org/licenses/lgpl-3.0.html |
| NumPy | array maths | BSD-3-Clause | https://numpy.org/ |
| SciPy | filtering, optimisation | BSD-3-Clause | https://scipy.org/ |
| OpenCV (opencv-python) | image operations | Apache-2.0 (OpenCV), packaging MIT | https://opencv.org/ |
| Astropy | FITS files, WCS, sky coordinates | BSD-3-Clause | https://www.astropy.org/ |
| Pillow | PNG / JPG files | HPND (Pillow licence) | https://python-pillow.org/ |
| OpenNGC (data file objects_ongc.json.gz) | names of sky objects | CC-BY-SA-4.0, (c) Mattia Verga and contributors | https://github.com/mattiaverga/OpenNGC |
| Exo 2 (font) | program font | SIL Open Font License 1.1, (c) Natanael Gama | https://fonts.google.com/specimen/Exo+2 |
| PyInstaller | builds QHC.exe | GPL-2.0 with exception for bundled programs | https://pyinstaller.org/ |

## Qt / PySide6 (LGPL)
QHC uses Qt for Python dynamically linked (the Qt libraries are separate files next to QHC.exe in the program folder). You may
replace them with your own build of the same version of PySide6 / Qt under the terms of the LGPL v3. The source code of
PySide6 and Qt is available at https://code.qt.io/ . /
QHC benutzt Qt for Python dynamisch gelinkt (die Qt-Bibliotheken liegen als eigene Dateien im Programmordner neben QHC.exe).
Sie dürfen sie unter den Bedingungen der LGPL v3 durch eine eigene Version von PySide6 / Qt ersetzen. Der Quellcode von
PySide6 und Qt ist unter https://code.qt.io/ verfügbar.

Note: this is why the folder version (`dist\QHC\`) is the recommended way to ship QHC; a single-file exe packs the Qt libraries
into one archive, which makes replacing them harder. / Deshalb ist die Ordner-Version (`dist\QHC\`) die empfohlene Weitergabe;
eine Einzeldatei-exe packt die Qt-Bibliotheken in ein Archiv, das Ersetzen wird dadurch schwerer.

## OpenNGC (CC-BY-SA-4.0)
The object catalogue used for sky object names is derived from OpenNGC by Mattia Verga et al., licensed CC-BY-SA-4.0
(https://creativecommons.org/licenses/by-sa/4.0/). The data file `objects_ongc.json.gz` is a converted extract; it may be
used further under the same license. This does not change the license of the QHC program itself. /
Der Objektkatalog für die Namen von Himmelsobjekten stammt von OpenNGC (Mattia Verga u. a., CC-BY-SA-4.0). Die Datei
`objects_ongc.json.gz` ist ein umgewandelter Auszug und darf unter derselben Lizenz weiterverwendet werden. Die Lizenz des
Programms QHC selbst bleibt davon unberührt.
