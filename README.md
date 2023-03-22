# EasyOCR
Instal EasyOCR using :
  !pip install easyocr

Install Streamlit using :
  !pip install streamlit

Create EasyOCR reader and pass the image to read text from the image :
   reader = easyocr.Reader(['en'])
   results = reader.readtext(image_path)

To establish SQL connection :
  conn = sqlite3.connect('details.db')
  c = conn.cursor()
  
Code to run streamlit app in Colab using port 80 :
  !streamlit run --server.port 80 app.py &>/dev/null&
  from pyngrok import ngrok 
  public_url = ngrok.connect(port='80')
  public_url
  
To terminate the runtime of streamlit app :
  !pgrep streamlit
  !ps -eaf | grep streamlit
  ngrok.kill()
     
