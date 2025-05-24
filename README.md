
app = Flask(__name__)

@app.route('/')
def stream():
    return send_file('video.mp4', mimetype='video/mp4')

if __name__ == '__main__':
    app.run(host='0.0.0.0', port=10000)
