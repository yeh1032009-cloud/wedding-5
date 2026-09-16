from flask import Flask, render_template_string

app = Flask(__name__)

# نضع كود HTML الخاص بالدعوة هنا
html_code = """
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <title>دعوة زفاف أحمد وسلمى</title>
</head>
<body>
    <h1>دعوة زفاف أحمد وسلمى</h1>
</body>
</html>
"""

@app.route('/')
def home():
    return render_template_string(html_code)

if __name__ == '__main__':
    app.run(debug=True)
    import sys
from PyQt5.QtWidgets import QApplication
from PyQt5.QtWebEngineWidgets import QWebEngineView

app = QApplication(sys.argv)
web = QWebEngineView()

# الكود الخاص بك يوضع هنا
html_content = """
<!-- انسخ كود الـ HTML الكامل هنا -->
"""

web.setHtml(html_content)
web.show()
sys.exit(app.exec_())
