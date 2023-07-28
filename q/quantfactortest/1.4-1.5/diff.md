# Comparing `tmp/quantfactortest-1.4.tar.gz` & `tmp/quantfactortest-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantfactortest-1.4.tar", last modified: Thu Jul 27 03:24:50 2023, max compression
+gzip compressed data, was "quantfactortest-1.5.tar", last modified: Fri Jul 28 03:08:59 2023, max compression
```

## Comparing `quantfactortest-1.4.tar` & `quantfactortest-1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 03:24:50.178553 quantfactortest-1.4/
--rw-rw-rw-   0        0        0     6701 2023-07-27 03:24:50.178553 quantfactortest-1.4/PKG-INFO
--rw-rw-rw-   0        0        0     6109 2023-07-27 03:23:34.000000 quantfactortest-1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 03:24:50.176728 quantfactortest-1.4/quantfactortest.egg-info/
--rw-rw-rw-   0        0        0     6701 2023-07-27 03:24:50.000000 quantfactortest-1.4/quantfactortest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-07-27 03:24:50.000000 quantfactortest-1.4/quantfactortest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 03:24:50.000000 quantfactortest-1.4/quantfactortest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-07-27 03:24:50.000000 quantfactortest-1.4/quantfactortest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-27 03:24:50.000000 quantfactortest-1.4/quantfactortest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    40097 2023-07-27 02:32:49.000000 quantfactortest-1.4/quantfactortest.py
--rw-rw-rw-   0        0        0       42 2023-07-27 03:24:50.178553 quantfactortest-1.4/setup.cfg
--rw-rw-rw-   0        0        0     1371 2023-07-27 03:23:49.000000 quantfactortest-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 03:08:59.093264 quantfactortest-1.5/
+-rw-rw-rw-   0        0        0     6701 2023-07-28 03:08:59.092267 quantfactortest-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6109 2023-07-27 03:23:34.000000 quantfactortest-1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 03:08:59.091288 quantfactortest-1.5/quantfactortest.egg-info/
+-rw-rw-rw-   0        0        0     6701 2023-07-28 03:08:59.000000 quantfactortest-1.5/quantfactortest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-07-28 03:08:59.000000 quantfactortest-1.5/quantfactortest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 03:08:59.000000 quantfactortest-1.5/quantfactortest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-07-28 03:08:59.000000 quantfactortest-1.5/quantfactortest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-28 03:08:59.000000 quantfactortest-1.5/quantfactortest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    39751 2023-07-28 03:07:37.000000 quantfactortest-1.5/quantfactortest.py
+-rw-rw-rw-   0        0        0       42 2023-07-28 03:08:59.093264 quantfactortest-1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1371 2023-07-28 03:07:55.000000 quantfactortest-1.5/setup.py
```

### Comparing `quantfactortest-1.4/PKG-INFO` & `quantfactortest-1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantfactortest
-Version: 1.4
+Version: 1.5
 Summary: 单因子的测试（日级别and分钟级别）,非交互式
 Home-page: https://github.com/Masteryeda
 Author: IDEA_Wenzhi
 Author-email: 1259429314@qq.com
 Maintainer: IDEA_Wenzhi
 Maintainer-email: 1259429314@qq.com
 License: MIT License
```

### Comparing `quantfactortest-1.4/README.md` & `quantfactortest-1.5/README.md`

 * *Files identical despite different names*

### Comparing `quantfactortest-1.4/quantfactortest.egg-info/PKG-INFO` & `quantfactortest-1.5/quantfactortest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantfactortest
-Version: 1.4
+Version: 1.5
 Summary: 单因子的测试（日级别and分钟级别）,非交互式
 Home-page: https://github.com/Masteryeda
 Author: IDEA_Wenzhi
 Author-email: 1259429314@qq.com
 Maintainer: IDEA_Wenzhi
 Maintainer-email: 1259429314@qq.com
 License: MIT License
```

### Comparing `quantfactortest-1.4/quantfactortest.py` & `quantfactortest-1.5/quantfactortest.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import scipy.stats as st
 import seaborn as sns
 from scipy.stats import pearsonr
 import matplotlib.ticker as ticker
 import warnings
 import baostock as bs
 warnings.filterwarnings("ignore")
-plt.rcParams['font.sans-serif'] = ['SimHei']  # 用来正常显示中文标签
 plt.rcParams['axes.unicode_minus'] = False  # 用来正常显示负号
  
 def process_bar(percent, start_str='', end_str='', total_length=0):
     bar = ''.join(["\033[31m%s\033[0m"%'   '] * int(percent * total_length)) + ''
     bar = '\r' + start_str + bar.ljust(total_length) + ' {:0>4.1f}%|'.format(percent*100) + end_str
     print(bar, end='', flush=True)
     
@@ -93,54 +92,53 @@
             total.append([])
         for i in range(len(self.factor)):
             now_row=sorted(list(self.factor.iloc[i]))
             for j in range(self.quantiles):
                 total[j]+=now_row[int(j*len(now_row)/self.quantiles):int((j+1)*len(now_row)/self.quantiles)]
         df=pd.DataFrame()
         for i in range(self.quantiles):
-            df['第'+str(i+1)+'分位']=total[i]
+            df['第'+str(i+1)+'分组']=total[i]
         print(df.describe(percentiles=percentiles).T)
         
     def set_picture(self):
         plt.xticks(fontsize=20)
         plt.yticks(fontsize=20)
         plt.legend(prop={'size':20})
     
     def group_picture(self,time_gap,factor):
         sns.set(palette="muted", color_codes=True)
-        sns.set(font='SimHei', font_scale=0.8)
         years=int(str(factor.index[len(factor)-1])[:4])-int(str(factor.index[0])[:4])+1
         months=[]
         for i in range(0,years):
             months.append([])
             for j in range(0,12):
                 months[i].append(0)
                 
                 
         fig, ax = plt.subplots(figsize=(30,20))         
         for i in range(0,self.quantiles):
-            ax.plot(factor.index.strftime('%Y-%m-%d'), self.group_total_return[i], label="第"+str(i+1)+'分位的累加收益率')
+            ax.plot(factor.index.strftime('%Y-%m-%d'), self.group_total_return[i], label="The "+str(i+1)+'the group')
         ax.legend(loc='best')
         ax.xaxis.set_major_locator(ticker.MultipleLocator(base=len(factor)/8))
-        plt.xlabel("时间",fontsize=16)
-        plt.ylabel("收益情况",fontsize=16)
+        plt.xlabel("Time",fontsize=20)
+        plt.ylabel("Return Rate",fontsize=20)
         self.set_picture()           
-        plt.title(str(time_gap)+'天收益周期的各分位的累加收益率',fontdict={'size': 20})  
+        plt.title(str(time_gap)+'day: Accumulated Return',fontdict={'size': 20})  
         plt.show()
         
         
         fig, ax = plt.subplots(figsize=(30,20))         
         for i in range(0,self.quantiles):
-            ax.plot(factor.index.strftime('%Y-%m-%d'), self.group_compound_return[i], label="第"+str(i+1)+'分位的复利累计收益率')
+            ax.plot(factor.index.strftime('%Y-%m-%d'), self.group_compound_return[i], label="The "+str(i+1)+'the group')
         ax.legend(loc='best')
         ax.xaxis.set_major_locator(ticker.MultipleLocator(base=len(factor)/8))
-        plt.xlabel("时间",fontsize=16)
-        plt.ylabel("收益情况",fontsize=16)
+        plt.xlabel("Time",fontsize=20)
+        plt.ylabel("Retun Rate",fontsize=20)
         self.set_picture()           
-        plt.title(str(time_gap)+'天收益周期的各分位的复利收益率',fontdict={'size': 20})  
+        plt.title(str(time_gap)+'day: Compounded Return',fontdict={'size': 24})  
         plt.show()
         
        
         ylist=[factor.index[0].year]
         current_year=factor.index[0].year
         for j in range(1,len(self.group_total_return[0])):
                 if current_year!=factor.index[j].year:
@@ -164,15 +162,15 @@
             xlist=['1','2','3','4','5','6','7','8','9','10','11','12']
             months=np.array(months)
             ax=sns.heatmap(months,mask=months==0,xticklabels=xlist,yticklabels=ylist,cmap='RdYlGn_r',annot=True,annot_kws={"fontsize":20})
             plt.xticks(fontsize=20)
             plt.yticks(fontsize=20)
             cbar = ax.collections[0].colorbar
             cbar.ax.tick_params(labelsize=20)
-            ax.set_title(str(time_gap)+'天收益周期的第'+str(i+1)+'分位的非复利月度收益图',fontdict={'size': 24})
+            ax.set_title(str(time_gap)+'days: the Accumulated Return of the '+str(i+1)+'th group',fontdict={'size': 24})
             plt.show()
                 
         for i in range(0,self.quantiles):
             fig, ax = plt.subplots(figsize=(30,20))
             current_rate=1
             current_time=factor.index[0]
             current_year=factor.index[0]
@@ -188,15 +186,15 @@
             xlist=['1','2','3','4','5','6','7','8','9','10','11','12']
             months=np.array(months)
             ax=sns.heatmap(months,mask=months==0,xticklabels=xlist,yticklabels=ylist,cmap='RdYlGn_r',annot=True,annot_kws={"fontsize":20})
             plt.xticks(fontsize=20)
             plt.yticks(fontsize=20)
             cbar = ax.collections[0].colorbar
             cbar.ax.tick_params(labelsize=20)
-            ax.set_title(str(time_gap)+'天收益周期的第'+str(i+1)+'分位的复利月度收益图',fontdict={'size': 24})
+            ax.set_title(str(time_gap)+'days: the Compouned Return of the '+str(i+1)+'th group',fontdict={'size': 24})
             plt.show()
                 
     def buy_and_sell(self,total_list,buy,sell,time_gap,factor):
         new_total=[]
         for i in range(len(total_list[0])):
             now=0
             for j in buy:
@@ -222,25 +220,24 @@
         df['策略收益率详情'][4]=victory_rate
         print()
         print(df.T)
         fig, ax = plt.subplots(figsize=(30,20))         
         ax.plot(factor.index.strftime('%Y-%m-%d'), self.group_compound_return, label="复利累计收益率")
         ax.legend(loc='best')
         ax.xaxis.set_major_locator(ticker.MultipleLocator(base=len(factor)/8))
-        plt.xlabel("时间",fontsize=16)
-        plt.ylabel("收益情况",fontsize=16)
+        plt.xlabel("Time",fontsize=20)
+        plt.ylabel("Return Rate",fontsize=20)
         self.set_picture()           
-        text=str(time_gap)+'天收益周期的做多'
+        text=str(time_gap)+'days: The Compouned Return of buying '
         for i in buy:
-            text+='第'+str(i+1)+'分位、'
-        text+='并做空'
+            text+='the '+str(i+1)+'th group, '
+        text+='and selling '
         for i in sell:
-            text+='第'+str(i+1)+'分位、'
-        text+='的复利收益率'
-        plt.title(text,fontdict={'size': 20})  
+            text+='the '+str(i+1)+'th group, '
+        plt.title(text,fontdict={'size': 24})  
         plt.show()
         
             
     def back_test(self,buy=[5],sell=[1]):
         buy[0]=min(self.quantiles,buy[0])
         for i in range(len(buy)):
             buy[i]-=1
@@ -307,15 +304,14 @@
             print()
             print(df.T)
             self.group_picture(time_gap,factor)
             self.buy_and_sell(total_list,buy,sell,time_gap,factor)
     
     def IC_value(self,gap=10):
         sns.set(palette="muted", color_codes=True)
-        sns.set(font='SimHei', font_scale=0.8)
         names=[]
         for i in self.periods:
             names.append('period_'+str(i))
 
         day_IC=pd.DataFrame(index=names)
         IC_mean=[]
         IC_std=[]
@@ -362,32 +358,32 @@
             Rank_std.append(np.std(RankIC))
             NormalRank.append(np.mean(RankIC)/np.std(RankIC))
             PRank.append(np.mean(P_RankIC_value))
             skRank.append(pd.Series(RankIC).skew())
             kurRank.append(pd.Series(RankIC).kurtosis())
             fig, ax = plt.subplots(figsize=(24,10))
             plt.ylim(-1.25, 1.25)
-            ax.plot(factor.index, IC, label='IC值折线图',alpha=0.3)
-            ax.plot(factor.index, pd.Series(IC).rolling(gap).mean(), label='IC值的'+str(gap)+'个时间单位的均值',color='g')
+            ax.plot(factor.index, IC, label='IC Value',alpha=0.3)
+            ax.plot(factor.index, pd.Series(IC).rolling(gap).mean(), label='The Mean Value of IC: rolling windows length is '+str(gap),color='darkgreen')
             ax.legend(loc='best')
-            plt.xlabel("时间",fontsize=16)
-            plt.ylabel("IC值",fontsize=16)
+            plt.xlabel("Time",fontsize=24)
+            plt.ylabel("IC Value",fontsize=24)
             self.set_picture()
-            plt.title(str(self.periods[i])+'天周期的IC值折线图',fontdict={'size': 20})
+            plt.title('The Line of IC Value: '+str(self.periods[i])+'days',fontdict={'size': 20})
             plt.show()
             
             fig, ax = plt.subplots(figsize=(24,10))
             plt.ylim(-1.25, 1.25)
-            ax.plot(factor.index, RankIC, label='RankIC值折线图',alpha=0.3)
-            ax.plot(factor.index, pd.Series(RankIC).rolling(gap).mean(), label='RankIC值的'+str(gap)+'个时间单位的均值',color='g')
+            ax.plot(factor.index, RankIC, label='RankIC Value',alpha=0.3)
+            ax.plot(factor.index, pd.Series(RankIC).rolling(gap).mean(), label='The Mean Value of RankIC: rolling windows length is '+str(gap),color='darkgreen')
             ax.legend(loc='best')
-            plt.xlabel("时间",fontsize=16)
-            plt.ylabel("IC值",fontsize=16)
+            plt.xlabel("Time",fontsize=24)
+            plt.ylabel("Rank IC Value",fontsize=24)
             self.set_picture()
-            plt.title(str(self.periods[i])+'天周期的RankIC值折线图',fontdict={'size': 20})
+            plt.title('The Line of Rank IC Value: '+str(self.periods[i])+'days',fontdict={'size': 20})
             plt.show()
             
         day_IC['IC Mean']=IC_mean 
         day_IC['IC Std.']=IC_std
         day_IC['IR']=NormalIR
         day_IC['p-value']=PIC
         day_IC['IC Skew']=skIC
@@ -464,15 +460,15 @@
     
     def get_all(self,percentiles=[0.2,0.4,0.6,0.8],buy=[5],sell=[1],gap=10):
         self.factor_statistic(percentiles)
         self.IC_value(gap)
         self.back_test(buy=buy,sell=sell)
         self.exchange_rate()
         self.self_corr()
-
+        pd.set_option('display.max_columns', 5)
         
 
 
 class analyze_minute_factor:
     def __init__(self,factor,price,minute,quantiles=5,periods=[240],demeaned=False,trade_day=[],trade_time=[]):
         factor.replace(np.inf,np.nan,inplace=True)
         factor.index=pd.to_datetime(factor.index)
@@ -562,50 +558,49 @@
     def set_picture(self):
         plt.xticks(fontsize=20)
         plt.yticks(fontsize=20)
         plt.legend(prop={'size':20})
     
     def group_picture(self,time_gap,factor,day):
         sns.set(palette="muted", color_codes=True)
-        sns.set(font='SimHei', font_scale=0.8)
         years=int(str(factor.index[len(factor)-1])[:4])-int(str(factor.index[0])[:4])+1
         months=[]
         for i in range(0,years):
             months.append([])
             for j in range(0,12):
                 months[i].append(0)
                 
                 
         fig, ax = plt.subplots(figsize=(30,20))         
         for i in range(0,self.quantiles):
-            ax.plot(factor.index.strftime('%Y-%m-%d %H:%M:%S'), self.group_total_return[i], label="第"+str(i+1)+'分位的累加收益率')
+            ax.plot(factor.index.strftime('%Y-%m-%d %H:%M:%S'), self.group_total_return[i], label="The "+str(i+1)+'the group')
         ax.legend(loc='best')
         ax.xaxis.set_major_locator(ticker.MultipleLocator(base=len(factor)/6))
-        plt.xlabel("时间",fontsize=16)
-        plt.ylabel("收益情况",fontsize=16)
+        plt.xlabel("Time",fontsize=20)
+        plt.ylabel("Return Rate",fontsize=20)
         self.set_picture()     
         if self.type=='K':
-            plt.title(str(time_gap)+'根K线收益周期的各分位的累加收益率',fontdict={'size': 20})  
+            plt.title(str(time_gap)+' K Line: Accumulated Return Rate',fontdict={'size': 24})  
         else:
-            plt.title('滞后'+str(self.trade_day[day])+'天在时刻'+self.trade_time[day]+'的各分位的累加收益率',fontdict={'size': 20})
+            plt.title('After '+str(self.trade_day[day])+'days at '+self.trade_time[day]+': Accumulated Return Rate',fontdict={'size': 20})
         plt.show()
         
         
         fig, ax = plt.subplots(figsize=(30,20))         
         for i in range(0,self.quantiles):
-            ax.plot(factor.index.strftime('%Y-%m-%d %H:%M:%S'), self.group_compound_return[i], label="第"+str(i+1)+'分位的复利累计收益率')
+            ax.plot(factor.index.strftime('%Y-%m-%d %H:%M:%S'), self.group_compound_return[i], label="The "+str(i+1)+'the group')
         ax.legend(loc='best')
         ax.xaxis.set_major_locator(ticker.MultipleLocator(base=len(factor)/6))
-        plt.xlabel("时间",fontsize=16)
-        plt.ylabel("收益情况",fontsize=16)
+        plt.xlabel("Time",fontsize=20)
+        plt.ylabel("Return Rate",fontsize=20)
         self.set_picture()   
         if self.type=='K':        
-            plt.title(str(time_gap)+'根K线收益周期的各分位的复利收益率',fontdict={'size': 20})
+            plt.title(str(time_gap)+' K Line: Compounded Return Rate',fontdict={'size': 24})
         else:
-            plt.title('滞后'+str(self.trade_day[day])+'天在时刻'+self.trade_time[day]+'的各分位的复利收益率',fontdict={'size': 20})
+            plt.title('After '+str(self.trade_day[day])+'days at '+self.trade_time[day]+': Compounded Return Rate',fontdict={'size': 24})
         plt.show()
         
                 
     def buy_and_sell(self,total_list,buy,sell,time_gap,factor,day):
         new_total=[]
         for i in range(len(total_list[0])):
             now=0
@@ -632,28 +627,27 @@
         df['策略收益率详情'][4]=victory_rate
         print()
         print(df.T)
         fig, ax = plt.subplots(figsize=(30,20))         
         ax.plot(factor.index.strftime('%Y-%m-%d %H:%M:%S'), self.group_compound_return, label="复利累计收益率")
         ax.legend(loc='best')
         ax.xaxis.set_major_locator(ticker.MultipleLocator(base=len(factor)/6))
-        plt.xlabel("时间",fontsize=16)
-        plt.ylabel("收益情况",fontsize=16)
+        plt.xlabel("Time",fontsize=20)
+        plt.ylabel("Return Rate",fontsize=20)
         self.set_picture()   
         if self.type=='K':        
-            text=str(time_gap)+'根K线收益周期的做多'
+            text='The Compounded Return of ' +str(time_gap)+'K Line: buy '
         else:
-            text='滞后'+str(self.trade_day[day])+'天在时刻'+self.trade_time[day]
+            text='After '+str(self.trade_day[day])+'days at '+self.trade_time[day]+': buy '
         for i in buy:
-            text+='第'+str(i+1)+'分位、'
-        text+='并做空'
+            text+='the '+str(i+1)+'the group,'
+        text+='and sell '
         for i in sell:
-            text+='第'+str(i+1)+'分位、'
-        text+='的复利收益率'
-        plt.title(text,fontdict={'size': 20})  
+            text+='the '+str(i+1)+'the group,'
+        plt.title(text,fontdict={'size': 24})  
         plt.show()
         
             
     def back_test(self,buy=[5],sell=[1]):
         buy[0]=min(self.quantiles,5)
         for i in range(len(buy)):
             buy[i]-=1
@@ -770,40 +764,40 @@
             Rank_std.append(np.std(RankIC))
             NormalRank.append(np.mean(RankIC)/np.std(RankIC))
             PRank.append(np.mean(P_RankIC_value))
             skRank.append(pd.Series(RankIC).skew())
             kurRank.append(pd.Series(RankIC).kurtosis())
             fig, ax = plt.subplots(figsize=(24,10))
             plt.ylim(-1.25, 1.25)
-            ax.plot(factor.index.strftime('%Y-%m-%d %H:%M:%S'), IC, label='IC值折线图',alpha=0.3)
-            ax.plot(factor.index.strftime('%Y-%m-%d %H:%M:%S'), pd.Series(IC).rolling(gap).mean(), label='IC值的'+str(gap)+'个时间单位的均值',color='g')
+            ax.plot(factor.index.strftime('%Y-%m-%d %H:%M:%S'), IC, label='IC Value',alpha=0.3)
+            ax.plot(factor.index.strftime('%Y-%m-%d %H:%M:%S'), pd.Series(IC).rolling(gap).mean(), label='The Mean Value of IC: rolling windows length is'+str(gap),color='darkgreen')
             ax.legend(loc='best')
-            plt.xlabel("时间",fontsize=16)
-            plt.ylabel("IC值",fontsize=16)
+            plt.xlabel("Time",fontsize=20)
+            plt.ylabel("IC Value",fontsize=20)
             ax.xaxis.set_major_locator(ticker.MultipleLocator(base=len(self.factor)/6))
             self.set_picture()
             if self.type=='K':
-                plt.title(str(self.periods[i])+'根K线周期的IC值折线图',fontdict={'size': 20})
+                plt.title(str(self.periods[i])+'K Line: IC Value',fontdict={'size': 20})
             else:
-                plt.title('滞后'+str(self.trade_day[i])+'天在时刻'+self.trade_time[i]+'的IC值折线图',fontdict={'size': 20})
+                plt.title('After '+str(self.trade_day[i])+'days at '+self.trade_time[i]+': IC Value',fontdict={'size': 20})
             plt.show()
             
             fig, ax = plt.subplots(figsize=(24,10))
             plt.ylim(-1.25, 1.25)
-            ax.plot(factor.index.strftime('%Y-%m-%d %H:%M:%S'), RankIC, label='RankIC值折线图',alpha=0.3)
-            ax.plot(factor.index.strftime('%Y-%m-%d %H:%M:%S'), pd.Series(RankIC).rolling(gap).mean(), label='RankIC值的'+str(gap)+'个时间单位的均值',color='g')
+            ax.plot(factor.index.strftime('%Y-%m-%d %H:%M:%S'), RankIC, label='RankIC Value',alpha=0.3)
+            ax.plot(factor.index.strftime('%Y-%m-%d %H:%M:%S'), pd.Series(RankIC).rolling(gap).mean(), label='The Mean Value of Rank IC: rolling windows length is'+str(gap),color='darkgreen')
             ax.legend(loc='best')
-            plt.xlabel("时间",fontsize=16)
-            plt.ylabel("IC值",fontsize=16)
+            plt.xlabel("Time",fontsize=20)
+            plt.ylabel("IC Value",fontsize=20)
             ax.xaxis.set_major_locator(ticker.MultipleLocator(base=len(self.factor)/6))
             self.set_picture()
             if self.type=='K':
-                plt.title(str(self.periods[i])+'根K线周期的RankIC值折线图',fontdict={'size': 20})
+                plt.title(str(self.periods[i])+'K Line: Rank IC Value',fontdict={'size': 20})
             else:
-                plt.title('滞后'+str(self.trade_day[i])+'天在时刻'+self.trade_time[i]+'的RankIC值折线图',fontdict={'size': 20})
+                plt.title('After '+str(self.trade_day[i])+'days at '+self.trade_time[i]+': Rank IC Value',fontdict={'size': 20})
             plt.show()
             
         day_IC['IC Mean']=IC_mean 
         day_IC['IC Std.']=IC_std
         day_IC['IR']=NormalIR
         day_IC['p-value']=PIC
         day_IC['IC Skew']=skIC
@@ -883,9 +877,9 @@
     
     def get_all(self,percentiles=[0.2,0.4,0.6,0.8],buy=[5],sell=[1],gap=10):
         self.factor_statistic(percentiles)
         self.IC_value(gap)
         self.back_test(buy,sell)
         self.exchange_rate()
         self.self_corr()
+        pd.set_option('display.max_columns', 5)
 
-
```

### Comparing `quantfactortest-1.4/setup.py` & `quantfactortest-1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
  
 setup(
     name='quantfactortest',#包名
-    version='1.4',#版本
+    version='1.5',#版本
     description="单因子的测试（日级别and分钟级别）,非交互式",#包简介
     long_description=open('README.md', encoding='utf-8').read(),#读取文件中介绍包的详细内容
     include_package_data=True,#是否允许上传资源文件
     author='IDEA_Wenzhi',#作者
     author_email='1259429314@qq.com',#作者邮件
     maintainer='IDEA_Wenzhi',#维护者
     maintainer_email='1259429314@qq.com',#维护者邮件
```

