from selenium import webdriver
import time as time
import sys
def login(credentials):
	username = credentials[1]
	password = credentials[2]
	driver = webdriver.Firefox()
	driver.get('https://wifilogin.myion.in/?page=login')
	driver.find_element_by_id('cpusername').send_keys(username)
	driver.find_element_by_id('cppassword').send_keys(password)
	driver.find_element_by_id('btnLogin').click()
	time.sleep(2)
	obj = driver.switch_to_alert()
	obj.accept()
	driver.close()

login(sys.argv)