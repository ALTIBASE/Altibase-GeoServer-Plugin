# Altibase-GeoServer-Plugin

Altibase를 GeoServer에 연동하기 위한 Plugin이다.
지원 버전: Altibase 7.1.0
          GeoServer 2.16


Altibase 7.1.0부터 Spatial에 다음과 같은 변화가 있다.
- GEOMETRY_COLUMNS와  SPATIAL_REF_SYS가 메타테이블로 변경됨
- GEOMETRY_COLUMNS은 자동으로 관리됨
- SPATIAL_REF_SYS은 시스템 프로시져를 사용해서만 설정할 수 있음
- SRID를 포함한 Extended WKT, Extended WKB 지원


이에 따라 mangosystem에서 제작한 이전 버전의 plugin(gt-jdbc-altibase-21-SNAPSHOT.jar)이
Altibase 7.1.0과 호환되지 않아 아래의 repository 소스를 일부 수정하여 gt-jdbc-altibase-22-SNAPSHOT.jar를 제공한다. 

mangosystem repository: https://github.com/mangosystem/geotools-jdbc-korean/tree/master/jdbc-altibase
