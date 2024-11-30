import pandas
get_info=input() 
fails = pandas.read_excel("description.xlsx", sheet_name="LookupAREA") 
info_list = fails.values.tolist()


info_list = fails.values.tolist()
get_info = input('Kāds reģions? ') or "Peria, Kaeo" 
reg_id = 0
for row in info_list:
    if row[1] == get_info:
        reg_id = row[0]
        break
if reg_id == 0:
    print('Reģions nav atrasts')
    exit()
print(reg_id)
CleanData = []
with open('data.csv', 'r') as csv:
    for line in csv:
        CleanData.append(line.rstrip().split(','))
geo_count = []
for line in CleanData:
    if line[1] == str(reg_id): 
        geo_count.append(int(line[3]))  
print(sum(geo_count))






