
# response = client.api.statuses. user_timeline. get (screen_name i. scre
print 'Got', len (response. data), 'tweets from', i.screen_name if len (response. data) != 0:
ltdate = response. data[0] ['created _at ']
ltdate2 = datetime.strptime(ltdate, '%a % %d SH:°M:85 +0000 gY'
today = datetime.now()
howlong = (today ltdate2) .days
if howlong < daywindow:
print i.screen_name, 'has tweeted in the past' , daywindow, totaltweets += len (response.data) for j in response. data: if j.entities.urls:
for k in j.entities.urls:
newurl = k['expanded url']
urlset.add( (newurl, j.user.screen_name) )
