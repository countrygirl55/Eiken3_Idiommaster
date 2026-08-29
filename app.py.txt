import streamlit as st
import streamlit.components.v1 as components

st.set_page_config(layout="wide", page_title="英検3級熟語マスター V22")

# 生成されたHTMLファイルを丸ごと読み込んで画面にロード
with open("eiken_3_idioms_quiz.html", "r", encoding="utf-8") as f:
    html_code = f.read()

components.html(html_code, height=900, scrolling=True)