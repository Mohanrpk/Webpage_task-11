# Webpage_task-11

from selenium import webdriver
from selenium.webdriver.common.by import By
from time import sleep
driver = webdriver.Chrome()

url = "https://www.saucedemo.com/"

driver.get(url)

driver.maximize_window()

sleep(2)

webelement_of_email_input = driver.find_element(By.NAME,"user-name")
webelement_of_email_input.send_keys("standard_user")

sleep(2)
