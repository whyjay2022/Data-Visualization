# Data-Visualization

import pandas as pd
import altair as alt

df = pd.read_csv('https://raw.githubusercontent.com/logistex/vd21/main/cctv_with_pop.csv')
offices = pd.read_csv('https://raw.githubusercontent.com/logistex/vd21/main/offices.csv')
seoul_url = 'https://raw.githubusercontent.com/southkorea/seoul-maps/master/juso/2015/json/seoul_municipalities_topo.json'
seoul = alt.topo_feature(seoul_url, 'seoul_municipalities_geo')

seoul
