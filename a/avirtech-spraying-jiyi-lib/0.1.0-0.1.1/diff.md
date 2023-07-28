# Comparing `tmp/avirtech_spraying_jiyi_lib-0.1.0.tar.gz` & `tmp/avirtech_spraying_jiyi_lib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avirtech_spraying_jiyi_lib-0.1.0.tar", last modified: Tue Jul 25 07:58:52 2023, max compression
+gzip compressed data, was "avirtech_spraying_jiyi_lib-0.1.1.tar", last modified: Fri Jul 28 00:14:07 2023, max compression
```

## Comparing `avirtech_spraying_jiyi_lib-0.1.0.tar` & `avirtech_spraying_jiyi_lib-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 07:58:52.674107 avirtech_spraying_jiyi_lib-0.1.0/
--rw-rw-rw-   0        0        0     1193 2023-07-25 07:58:52.673106 avirtech_spraying_jiyi_lib-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      423 2023-07-24 08:58:08.000000 avirtech_spraying_jiyi_lib-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 07:58:52.663130 avirtech_spraying_jiyi_lib-0.1.0/avirtech_spraying_jiyi_lib/
--rw-rw-rw-   0        0        0       47 2023-07-24 08:46:59.000000 avirtech_spraying_jiyi_lib-0.1.0/avirtech_spraying_jiyi_lib/__init__.py
--rw-rw-rw-   0        0        0    31451 2023-07-25 07:51:26.000000 avirtech_spraying_jiyi_lib-0.1.0/avirtech_spraying_jiyi_lib/avirtech_spraying_jiyi.py
-drwxrwxrwx   0        0        0        0 2023-07-25 07:58:52.672134 avirtech_spraying_jiyi_lib-0.1.0/avirtech_spraying_jiyi_lib.egg-info/
--rw-rw-rw-   0        0        0     1193 2023-07-25 07:58:51.000000 avirtech_spraying_jiyi_lib-0.1.0/avirtech_spraying_jiyi_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      359 2023-07-25 07:58:52.000000 avirtech_spraying_jiyi_lib-0.1.0/avirtech_spraying_jiyi_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 07:58:51.000000 avirtech_spraying_jiyi_lib-0.1.0/avirtech_spraying_jiyi_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-07-25 07:58:52.000000 avirtech_spraying_jiyi_lib-0.1.0/avirtech_spraying_jiyi_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-07-25 07:58:52.000000 avirtech_spraying_jiyi_lib-0.1.0/avirtech_spraying_jiyi_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 07:58:52.675101 avirtech_spraying_jiyi_lib-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1422 2023-07-25 07:55:48.000000 avirtech_spraying_jiyi_lib-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 00:14:07.807925 avirtech_spraying_jiyi_lib-0.1.1/
+-rw-rw-rw-   0        0        0     1391 2023-07-28 00:14:07.806849 avirtech_spraying_jiyi_lib-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      617 2023-07-28 00:10:45.000000 avirtech_spraying_jiyi_lib-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 00:14:07.763965 avirtech_spraying_jiyi_lib-0.1.1/avirtech_spraying_jiyi_lib/
+-rw-rw-rw-   0        0        0       47 2023-07-24 08:46:59.000000 avirtech_spraying_jiyi_lib-0.1.1/avirtech_spraying_jiyi_lib/__init__.py
+-rw-rw-rw-   0        0        0    28021 2023-07-27 23:59:11.000000 avirtech_spraying_jiyi_lib-0.1.1/avirtech_spraying_jiyi_lib/avirtech_spraying_jiyi.py
+drwxrwxrwx   0        0        0        0 2023-07-28 00:14:07.804114 avirtech_spraying_jiyi_lib-0.1.1/avirtech_spraying_jiyi_lib.egg-info/
+-rw-rw-rw-   0        0        0     1391 2023-07-28 00:14:06.000000 avirtech_spraying_jiyi_lib-0.1.1/avirtech_spraying_jiyi_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      359 2023-07-28 00:14:07.000000 avirtech_spraying_jiyi_lib-0.1.1/avirtech_spraying_jiyi_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 00:14:06.000000 avirtech_spraying_jiyi_lib-0.1.1/avirtech_spraying_jiyi_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-07-28 00:14:06.000000 avirtech_spraying_jiyi_lib-0.1.1/avirtech_spraying_jiyi_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-07-28 00:14:06.000000 avirtech_spraying_jiyi_lib-0.1.1/avirtech_spraying_jiyi_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 00:14:07.807925 avirtech_spraying_jiyi_lib-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1422 2023-07-28 00:12:55.000000 avirtech_spraying_jiyi_lib-0.1.1/setup.py
```

### Comparing `avirtech_spraying_jiyi_lib-0.1.0/PKG-INFO` & `avirtech_spraying_jiyi_lib-0.1.1/avirtech_spraying_jiyi_lib.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: avirtech_spraying_jiyi_lib
-Version: 0.1.0
+Name: avirtech-spraying-jiyi-lib
+Version: 0.1.1
 Summary: Avirtech Python Library to Generate drone spraying error with palm location
 Home-page: 
 Author: Mohammad ILham R
 Author-email: ilhamr.mohammad@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -16,15 +16,19 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 Script ini untuk membuat jalurterbang Spraying untuk drone spraying FC JIYI.
 Data yang dihasilkan adalah berupa garis(.shp).
-Data tersebut dilanjutkan di software Qgis, untuk diconvert menjadi (.kml) lalu di "dissolve".
+Data garis(.shp) yang diperlukan menggunakan koordinat WGS_1984, Mohon tidak diproject ke UTM.
+Bila menggunakan data DSM(.tif) boleh menggunakan koordinat WGS_1984, maupun koordinat UTM.
+
+
+Data tersebut dilanjutkan di software Qgis, untuk diconvert menjadi (.kml), lalu di "dissolve".
 Data hasil dissolve dapat digunakan dalam aplikasi "AgriAsistant"
 
 Install
 pip install avirtech_spraying_jiyi_lib
 
 Usage
 from avirtech_spraying_jiyi_lib.avirtech_spraying_jiyi import autocorrect
```

### Comparing `avirtech_spraying_jiyi_lib-0.1.0/avirtech_spraying_jiyi_lib/avirtech_spraying_jiyi.py` & `avirtech_spraying_jiyi_lib-0.1.1/avirtech_spraying_jiyi_lib/avirtech_spraying_jiyi.py`

 * *Files 23% similar despite different names*

```diff
@@ -235,28 +235,28 @@
                     data_csv.append(os.path.join(lokasi_output_folder, file))
 
             output_keluaran = os.path.join(lokasi_output_folder, "output_keluaran")
             os.mkdir(output_keluaran)
 
 
             # Process: Make XY Event Layer
-            arcpy.MakeXYEventLayer_management(data_csv[0], "POINT_X", "POINT_Y", 'z_layer_xy_point_shp', "PROJCS['WGS_1984_UTM_Zone_48S',GEOGCS['GCS_WGS_1984',DATUM['D_WGS_1984',SPHEROID['WGS_1984',6378137.0,298.257223563]],PRIMEM['Greenwich',0.0],UNIT['Degree',0.0174532925199433]],PROJECTION['Transverse_Mercator'],PARAMETER['False_Easting',500000.0],PARAMETER['False_Northing',10000000.0],PARAMETER['Central_Meridian',105.0],PARAMETER['Scale_Factor',0.9996],PARAMETER['Latitude_Of_Origin',0.0],UNIT['Meter',1.0]];-5120900 1900 10000;-100000 10000;-100000 10000;0,001;0,001;0,001;IsHighPrecision", "")
+            arcpy.MakeXYEventLayer_management(data_csv[0], "POINT_X", "POINT_Y", 'z_layer_xy_point_shp', "GEOGCS['GCS_WGS_1984',DATUM['D_WGS_1984',SPHEROID['WGS_1984',6378137.0,298.257223563]],PRIMEM['Greenwich',0.0],UNIT['Degree',0.0174532925199433]];-400 -400 1000000000;-100000 10000;-100000 10000;8,98315284119522E-09;0,001;0,001;IsHighPrecision", "")
 
             # Process: Feature Class To Shapefile (multiple)
             arcpy.FeatureClassToShapefile_conversion("'z_layer_xy_point_shp'", output_keluaran)
 
             data_ptcsv = []
             for file in os.listdir(output_keluaran):
                 if file.endswith('.shp'):
                     data_ptcsv.append(os.path.join(output_keluaran, file))
 
             # Process: Add Attribute Index
             arcpy.AddIndex_management(data_ptcsv[0], "Id", "", "NON_UNIQUE", "NON_ASCENDING")
 
-            arcpy.XYToLine_management(data_csv[0], os.path.join(output_keluaran, "ln_ready_to_3d.shp"), "start_x", "start_y", "end_x2", "end_y2", "0", "Id", "PROJCS['WGS_1984_UTM_Zone_48S',GEOGCS['GCS_WGS_1984',DATUM['D_WGS_1984',SPHEROID['WGS_1984',6378137.0,298.257223563]],PRIMEM['Greenwich',0.0],UNIT['Degree',0.0174532925199433]],PROJECTION['Transverse_Mercator'],PARAMETER['False_Easting',500000.0],PARAMETER['False_Northing',10000000.0],PARAMETER['Central_Meridian',105.0],PARAMETER['Scale_Factor',0.9996],PARAMETER['Latitude_Of_Origin',0.0],UNIT['Meter',1.0]];-5120900 1900 450445547,391054;-100000 10000;-100000 10000;0,001;0,001;0,001;IsHighPrecision")
+            arcpy.XYToLine_management(data_csv[0], os.path.join(output_keluaran, "ln_ready_to_3d.shp"), "start_x", "start_y", "end_x2", "end_y2", "0", "Id", "GEOGCS['GCS_WGS_1984',DATUM['D_WGS_1984',SPHEROID['WGS_1984',6378137.0,298.257223563]],PRIMEM['Greenwich',0.0],UNIT['Degree',0.0174532925199433]];-400 -400 1000000000;-100000 10000;-100000 10000;8,98315284119522E-09;0,001;0,001;IsHighPrecision")
 
             # Process: Add Attribute Index
             arcpy.AddIndex_management(data_line_split[0], "Id", "", "NON_UNIQUE", "NON_ASCENDING")
             # Process: Add Attribute Index
             arcpy.AddIndex_management(os.path.join(output_keluaran, "ln_ready_to_3d.shp"), "Id", "", "NON_UNIQUE", "NON_ASCENDING")
 
             data_ptcsv_scan2 = []
@@ -336,32 +336,14 @@
             colomn_tabel = colomn_tabel.drop(['end_dsm'], axis=1)
             colomn_tabel['selisih'] = (colomn_tabel['RASTERVALU'] - colomn_tabel['end_dsm2']).abs()
             colomn_tabel = colomn_tabel[["Id", "RASTERVALU", "selisih", "Tinggi Terbang", "POINT_X", "POINT_Y", "start_x", "end_x2", "start_y", "end_y2"]]
             colomn_tabel.columns = ["no_titik", "DSM", "Selisih", "Tinggi Terbang", "POINT_X", "POINT_Y", "start_x", "end_x2", "start_y", "end_y2"]
 
             # colomn_tabel.to_csv(os.path.join(lokasi_folder,'final_dbf_siap_to_SCRIPTmasREY_satu.csv'))
             ''''''
-            fig, ax = plt.subplots()
-            ax2 = ax.twinx()
-
-            ax.plot(colomn_tabel['no_titik'], colomn_tabel['Tinggi Terbang'], 'ro', color='blue', markersize='2')
-            ax.xaxis.set_major_locator(MultipleLocator(150))
-            ax2.plot(colomn_tabel['no_titik'], colomn_tabel['Selisih'], color='grey',alpha=0.2)
-            ax2.set_ylabel('Selisih Ketinggian', fontsize=15)
-            ax2.set_ylim([0, 5])
-            ax.set_ylabel('Ketinggian', fontsize=15)
-            ax.set_xlabel('No titik', fontsize=15)
-            ax.grid(True)
-            ax.plot(colomn_tabel['no_titik'], colomn_tabel['DSM'], color='red', alpha=0.8)
-            # plt.plot(colomn_tabel['no_titik'])
-            ax.legend(loc= 2, fontsize="small")
-            # ax2.legend(loc= "upper right")
-            plt.gcf().set_size_inches((18,10))
-            plt.title("Scatter Plot Titik DSM, Tinggi Terbang, ", fontsize=20)
-            # plt.show()
 
             colomn_tabel.columns = [["Id", "RASTERVALU", "Selisih","Tinggi_Terbang", "POINT_X", "POINT_Y", "start_x", "end_x2", "start_y", "end_y2"]]
             colomn_tabel = colomn_tabel.drop(['Selisih'], axis=1)
 
             df = colomn_tabel
 
             ''' '''
@@ -392,28 +374,28 @@
                     data_csv.append(os.path.join(lokasi_output_folder, file))
 
             output_keluaran = os.path.join(lokasi_output_folder, "output_keluaran")
             os.mkdir(output_keluaran)
 
 
             # Process: Make XY Event Layer
-            arcpy.MakeXYEventLayer_management(data_csv[0], "POINT_X", "POINT_Y", 'z_layer_xy_point_shp', "PROJCS['WGS_1984_UTM_Zone_48S',GEOGCS['GCS_WGS_1984',DATUM['D_WGS_1984',SPHEROID['WGS_1984',6378137.0,298.257223563]],PRIMEM['Greenwich',0.0],UNIT['Degree',0.0174532925199433]],PROJECTION['Transverse_Mercator'],PARAMETER['False_Easting',500000.0],PARAMETER['False_Northing',10000000.0],PARAMETER['Central_Meridian',105.0],PARAMETER['Scale_Factor',0.9996],PARAMETER['Latitude_Of_Origin',0.0],UNIT['Meter',1.0]];-5120900 1900 10000;-100000 10000;-100000 10000;0,001;0,001;0,001;IsHighPrecision", "")
+            arcpy.MakeXYEventLayer_management(data_csv[0], "POINT_X", "POINT_Y", 'z_layer_xy_point_shp', "GEOGCS['GCS_WGS_1984',DATUM['D_WGS_1984',SPHEROID['WGS_1984',6378137.0,298.257223563]],PRIMEM['Greenwich',0.0],UNIT['Degree',0.0174532925199433]];-400 -400 1000000000;-100000 10000;-100000 10000;8,98315284119522E-09;0,001;0,001;IsHighPrecision", "")
 
             # Process: Feature Class To Shapefile (multiple)
             arcpy.FeatureClassToShapefile_conversion("'z_layer_xy_point_shp'", output_keluaran)
 
             data_ptcsv = []
             for file in os.listdir(output_keluaran):
                 if file.endswith('.shp'):
                     data_ptcsv.append(os.path.join(output_keluaran, file))
 
             # Process: Add Attribute Index
             arcpy.AddIndex_management(data_ptcsv[0], "Id", "", "NON_UNIQUE", "NON_ASCENDING")
 
-            arcpy.XYToLine_management(data_csv[0], os.path.join(output_keluaran, "ln_ready_to_3d.shp"), "start_x", "start_y", "end_x2", "end_y2", "0", "Id", "PROJCS['WGS_1984_UTM_Zone_48S',GEOGCS['GCS_WGS_1984',DATUM['D_WGS_1984',SPHEROID['WGS_1984',6378137.0,298.257223563]],PRIMEM['Greenwich',0.0],UNIT['Degree',0.0174532925199433]],PROJECTION['Transverse_Mercator'],PARAMETER['False_Easting',500000.0],PARAMETER['False_Northing',10000000.0],PARAMETER['Central_Meridian',105.0],PARAMETER['Scale_Factor',0.9996],PARAMETER['Latitude_Of_Origin',0.0],UNIT['Meter',1.0]];-5120900 1900 450445547,391054;-100000 10000;-100000 10000;0,001;0,001;0,001;IsHighPrecision")
+            arcpy.XYToLine_management(data_csv[0], os.path.join(output_keluaran, "ln_ready_to_3d.shp"), "start_x", "start_y", "end_x2", "end_y2", "0", "Id", "GEOGCS['GCS_WGS_1984',DATUM['D_WGS_1984',SPHEROID['WGS_1984',6378137.0,298.257223563]],PRIMEM['Greenwich',0.0],UNIT['Degree',0.0174532925199433]];-400 -400 1000000000;-100000 10000;-100000 10000;8,98315284119522E-09;0,001;0,001;IsHighPrecision")
 
             # Process: Add Attribute Index
             arcpy.AddIndex_management(data_line_split[0], "Id", "", "NON_UNIQUE", "NON_ASCENDING")
             # Process: Add Attribute Index
             arcpy.AddIndex_management(os.path.join(output_keluaran, "ln_ready_to_3d.shp"), "Id", "", "NON_UNIQUE", "NON_ASCENDING")
 
             data_ptcsv_scan2 = []
@@ -430,25 +412,23 @@
             arcpy.AddField_management("ln_ready_to_3d", "end_elv", "FLOAT", "", "", "", "", "NULLABLE", "NON_REQUIRED", "")
 
             arcpy.CalculateField_management("ln_ready_to_3d", "start_elv", "float(!start_elev!)", "PYTHON", "")
             arcpy.CalculateField_management("ln_ready_to_3d", "end_elv", "float(!end_elev2!)", "PYTHON", "")
 
             arcpy.management.CopyFeatures("ln_ready_to_3d", os.path.join(lokasi_output_folder,"ln_ready_to_3d_fixx.shp"))
 
-            arcpy.FeatureTo3DByAttribute_3d("ln_ready_to_3d_fixx", "3d_jalur_terbang.shp", "start_elv", "end_elv")
+            arcpy.FeatureTo3DByAttribute_3d("ln_ready_to_3d_fixx", os.path.join(lokasi_output_folder,"3d_jalur_terbang.shp"), "start_elv", "end_elv")
 
             arcpy.management.CopyFeatures("3d_jalur_terbang", os.path.join(lokasi_output,"3d_jalur_terbang_fixxx"))
 
         def local_altitude ():
             
-            
             lokasi_output_folder = os.path.join(lokasi_output, "lokasi_output")
             os.mkdir(lokasi_output_folder)
 
-
             data_jalur_terbang = []
             for file in os.listdir(lokasi_dsm_shp):
                 if file.endswith('.shp'):
                     data_jalur_terbang.append(os.path.join(lokasi_dsm_shp, file))
 
 
             arcpy.FeatureVerticesToPoints_management(data_jalur_terbang[0], os.path.join(lokasi_output_folder, 'pt_vertice_pohon.shp'), "ALL")
@@ -490,51 +470,31 @@
             colomn_tabel["end_dsm"] = colomn_tabel.iloc[1:, :].loc[:, 'ketinggian']
             colomn_tabel["end_dsm2"] = colomn_tabel['end_dsm'].shift(periods=-1)
             colomn_tabel = colomn_tabel.drop(['end_dsm'], axis=1)
             colomn_tabel['selisih'] = (colomn_tabel['ketinggian'] - colomn_tabel['end_dsm2']).abs()
             colomn_tabel = colomn_tabel[["Id", "ketinggian", "selisih", "Tinggi Terbang", "POINT_X", "POINT_Y", "start_x", "end_x2", "start_y", "end_y2"]]
             colomn_tabel.columns = ["no_titik", "DSM", "Selisih", "Tinggi Terbang", "POINT_X", "POINT_Y", "start_x", "end_x2", "start_y", "end_y2"]
 
-
             ''''''
-            fig, ax = plt.subplots()
-            ax2 = ax.twinx()
-            ax.plot(colomn_tabel['no_titik'], colomn_tabel['Tinggi Terbang'], 'ro', color='blue', markersize='2')
-            ax.xaxis.set_major_locator(MultipleLocator(150))
-            ax2.plot(colomn_tabel['no_titik'], colomn_tabel['Selisih'], color='grey',alpha=0.2)
-            ax2.set_ylabel('Selisih Ketinggian', fontsize=15)
-            ax2.set_ylim([0, 5])
-            ax.set_ylabel('Ketinggian', fontsize=15)
-            ax.set_xlabel('No titik', fontsize=15)
-            ax.grid(True)
-            ax.plot(colomn_tabel['no_titik'], colomn_tabel['DSM'], color='red', alpha=0.8)
-            # plt.plot(colomn_tabel['no_titik'])
-            ax.legend(loc= 2, fontsize="small")
-            # ax2.legend(loc= "upper right")
-            plt.gcf().set_size_inches((18,10))
-            plt.title("Scatter Plot Titik DSM, Tinggi Terbang, ", fontsize=20)
-            # plt.show()
-
+        
             colomn_tabel.columns = [["Id", "ketinggian", "Selisih","Tinggi_Terbang", "POINT_X", "POINT_Y", "start_x", "end_x2", "start_y", "end_y2"]]
             colomn_tabel = colomn_tabel.drop(['Selisih'], axis=1)
-
             df = colomn_tabel
 
             ''' '''
             df['start_elev'] = df['ketinggian']
             df['end_elev'] = df.iloc[1:, :].loc[:, 'start_elev']
             df['end_elev2'] = df['end_elev'].shift(periods=-1)
             df = df.drop(['end_elev'], axis=1)
             df.at[len(df)-1, 'end_elev2'] = ketinggiane_akhir
             df2 = df
             # print(df2.tail(10))
 
             df2.to_csv(os.path.join(lokasi_output_folder,'final_dbf_siap_to_SCRIPTmasREY.csv')) 
 
-
             data_line_split = []
             for file in os.listdir(lokasi_output_folder):
                 if 'pt_vertice_pohon.shp' in file:
                     data_line_split.append(os.path.join(lokasi_output_folder, file))
 
             data_csv = []
             for file in os.listdir(lokasi_output_folder):
@@ -542,28 +502,28 @@
                     data_csv.append(os.path.join(lokasi_output_folder, file))
 
             output_keluaran = os.path.join(lokasi_output_folder, "output_keluaran")
             os.mkdir(output_keluaran)
 
 
             # Process: Make XY Event Layer
-            arcpy.MakeXYEventLayer_management(data_csv[0], "POINT_X", "POINT_Y", 'z_layer_xy_point_shp', "PROJCS['WGS_1984_UTM_Zone_48S',GEOGCS['GCS_WGS_1984',DATUM['D_WGS_1984',SPHEROID['WGS_1984',6378137.0,298.257223563]],PRIMEM['Greenwich',0.0],UNIT['Degree',0.0174532925199433]],PROJECTION['Transverse_Mercator'],PARAMETER['False_Easting',500000.0],PARAMETER['False_Northing',10000000.0],PARAMETER['Central_Meridian',105.0],PARAMETER['Scale_Factor',0.9996],PARAMETER['Latitude_Of_Origin',0.0],UNIT['Meter',1.0]];-5120900 1900 10000;-100000 10000;-100000 10000;0,001;0,001;0,001;IsHighPrecision", "")
+            arcpy.MakeXYEventLayer_management(data_csv[0], "POINT_X", "POINT_Y", 'z_layer_xy_point_shp', "GEOGCS['GCS_WGS_1984',DATUM['D_WGS_1984',SPHEROID['WGS_1984',6378137.0,298.257223563]],PRIMEM['Greenwich',0.0],UNIT['Degree',0.0174532925199433]];-400 -400 1000000000;-100000 10000;-100000 10000;8,98315284119522E-09;0,001;0,001;IsHighPrecision", "")
 
             # Process: Feature Class To Shapefile (multiple)
             arcpy.FeatureClassToShapefile_conversion("'z_layer_xy_point_shp'", output_keluaran)
 
             data_ptcsv = []
             for file in os.listdir(output_keluaran):
                 if file.endswith('.shp'):
                     data_ptcsv.append(os.path.join(output_keluaran, file))
 
             # Process: Add Attribute Index
             arcpy.AddIndex_management(data_ptcsv[0], "Id", "", "NON_UNIQUE", "NON_ASCENDING")
 
-            arcpy.XYToLine_management(data_csv[0], os.path.join(output_keluaran, "ln_ready_to_3d.shp"), "start_x", "start_y", "end_x2", "end_y2", "0", "Id", "PROJCS['WGS_1984_UTM_Zone_48S',GEOGCS['GCS_WGS_1984',DATUM['D_WGS_1984',SPHEROID['WGS_1984',6378137.0,298.257223563]],PRIMEM['Greenwich',0.0],UNIT['Degree',0.0174532925199433]],PROJECTION['Transverse_Mercator'],PARAMETER['False_Easting',500000.0],PARAMETER['False_Northing',10000000.0],PARAMETER['Central_Meridian',105.0],PARAMETER['Scale_Factor',0.9996],PARAMETER['Latitude_Of_Origin',0.0],UNIT['Meter',1.0]];-5120900 1900 450445547,391054;-100000 10000;-100000 10000;0,001;0,001;0,001;IsHighPrecision")
+            arcpy.XYToLine_management(data_csv[0], os.path.join(output_keluaran, "ln_ready_to_3d.shp"), "start_x", "start_y", "end_x2", "end_y2", "0", "Id", "GEOGCS['GCS_WGS_1984',DATUM['D_WGS_1984',SPHEROID['WGS_1984',6378137.0,298.257223563]],PRIMEM['Greenwich',0.0],UNIT['Degree',0.0174532925199433]];-400 -400 1000000000;-100000 10000;-100000 10000;8,98315284119522E-09;0,001;0,001;IsHighPrecision")
 
             # Process: Add Attribute Index
             arcpy.AddIndex_management(data_line_split[0], "Id", "", "NON_UNIQUE", "NON_ASCENDING")
             # Process: Add Attribute Index
             arcpy.AddIndex_management(os.path.join(output_keluaran, "ln_ready_to_3d.shp"), "Id", "", "NON_UNIQUE", "NON_ASCENDING")
 
             data_ptcsv_scan2 = []
@@ -590,8 +550,8 @@
             
         if output1 == "Flat Altitude":
             flat_altitude()
         elif output1 == "Adding DSM Altitude":
             dsm_altitude()
         elif output1 == "Adding Local Altitude":
             local_altitude()
-# autocorrect.process_all()
+autocorrect.process_all()
```

### Comparing `avirtech_spraying_jiyi_lib-0.1.0/setup.py` & `avirtech_spraying_jiyi_lib-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup( 
     name="avirtech_spraying_jiyi_lib",
-    version="0.1.0",
+    version="0.1.1",
     description="Avirtech Python Library to Generate drone spraying error with palm location",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="Mohammad ILham R",
     author_email="ilhamr.mohammad@gmail.com",
     license="MIT",
```

