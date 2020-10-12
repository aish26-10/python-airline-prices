#beginning of code
import time
from selenium import webdriver

browser = webdriver.Firefox(executable_path=r'C:\Users\aishr\Downloads\geckodriver-v0.26.0-win64\geckodriver.exe')
browser.get('https://www.travelocity.com/')

time.sleep(1)
# Click for flights
browser.find_element_by_xpath('//*[@id="tab-flight-tab-hp"]/span[1]').click()

time.sleep(1)
# Set origin
origin = browser.find_element_by_xpath('//*[@id="flight-origin-hp-flight"]')
origin.clear()
origin.send_keys("Chicago, IL (ORD-O'Hare Intl.)")

# Set destination
time.sleep(1)
dest = browser.find_element_by_xpath('//*[@id="flight-destination-hp-flight"]')
dest.clear()
dest.send_keys("Mumbai, India (BOM-Chhatrapati Shivaji Intl.)")

# Set departure date
time.sleep(1)
ddate = browser.find_element_by_xpath('//*[@id="flight-departing-hp-flight"]')
ddate.clear()
ddate.send_keys("12/16/2019")

# Set return date
time.sleep(1)
rdate = browser.find_element_by_xpath('//*[@id="flight-returning-hp-flight"]')
rdate.clear()
browser.find_element_by_xpath('//*[@id="flight-returning-hp-flight"]').click()
browser.find_element_by_xpath('//*[@id="flight-returning-wrapper-hp-flight"]/div/div/button[2]').click()
browser.find_element_by_xpath('/html/body/meso-native-marquee/section/div/div/div[1]/div/div/div[1]/div/section[1]/form/fieldset[2]/div[1]/div[3]/div/div/div/div[3]/table/tbody/tr[2]/td[6]/button').click()

# Click search
browser.find_element_by_xpath('//*[@id="gcw-flights-form-hp-flight"]/div[8]/label/button').click()

# Capture price
time.sleep(10)
price=browser.find_element_by_xpath('/html/body/div[2]/div[10]/section/div/div[10]/ul/li[1]/div[1]/div[1]/div[2]/div/div[1]/div[1]/span')
print(price.text)
#End of Code
