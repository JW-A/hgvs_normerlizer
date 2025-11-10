# hgvs_normerlizer

python3 -m pip install hgvsnorm-cli-0.2.2.tar.gz \

hgvsnorm --excel-in "/path/to/minimal_maf_test.xlsx" \
         --sheet 0 \
         --excel-out "/path/to/minimal_maf_test.normalized.xlsx" \
         --threads 16


# 기능 요약
- 여러 방식으로 쓰여지는 mutation 명명법을 HGVS로 통일
- 기본적으로 HGVSc, HGVSp, HGVSp_short에 작동하며 가능하다면 서로를 보완적으로 인식하고 채움
- 각각 명명법이 통일 되지 못한경우(323G>A, P.G125D... 등) 표준화된 HGVS 명명법으로 변경

