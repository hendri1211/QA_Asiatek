from selenium import webdriver
from selenium.webdriver.common.by import By
driver = webdriver.Chrome()
import time

#Test Case Registration Page


driver.get("https://myih.telkom.co.id/home")
driver.get("https://myih.telkom.co.id/register/account-details")

#entering nama lengkap
driver.find_element(By.XPATH,'//*[@id="nama lengkap"]/div/button').send_keys("hendri mardani")
#entering nomor ponsel
driver.find_element(By.XPATH,'//*[@id="naomor ponsel"]/div/button').send_keys("08117520666")
#enterinf email address
driver.find_element(By.XPATH,'//*[@id="email"]/div/button').send_keys("hendri.mardani@gmail.com")
#entering password   
driver.find_element_by_id("kata sandi").send_keys("Hendri1211")
#entering daftar sekarang button
driver.find_element_by_id(("submitbtn")).submit()



#driver.find_element_by_id("username").send_keys("test")
#driver.find_element_by_id("username").send_keys("test")
#driver.find_element_by_id("username").send_keys("test")
#driver.find_element_by_id("username").send_keys("test")

