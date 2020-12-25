# lammps_education_flow_win


# Note: This is test version. (Please, you would develop them)


In Mg, Al, Ca, Zr, etc., the molecule will be broken unless it is an oxidized surface with low reactivity.


------------------------------------------------------------------------------
■ lammps


□ インストール方法
1. http://packages.lammps.org/windows.html のHPで"64-bit Windows download area"をクリックする
2. LAMMPS-64bit-18Jun2019.exe をダウンロードして解凍する
3. ディフォルトの設定のまま最後まで進めばよい
以上で lammps のダウンロードと設定は完了です


□ 描画ソフト
 ・gnuplot（http://www.gnuplot.info/）
  http://www.yamamo10.jp/yamamoto/comp/gnuplot/inst_win/index.php
・Ovito（https://www.ovito.org/windows-downloads/）
※ web上に情報がありますので、お手数をおかけしますが、そちらをご参照ください
※ gnuplotのインストールと環境設定 (Edit: Dec/11/2020)
1. gnuplot - Browse /gnuplot at SourceForge.net から gp528-win64-mingw.exe を得る
  gp528-win64-mingw.exe をダブルクリック。設定はディフォルトのままでよい
2. コントロール パネル > システムとセキュリティ > システム
3. システムの環境設定 > 環境変数（N）... > システム環境変数（S）のPath > 編集（I）... > 新規（N）> C:\Program Files\gnuplot\bin を追加する > OK > OK
------------------------------------------------------------------------------
■ 分子動力学シミュレーション


□ 入力ファイルのダウンロード
  by-student-2017 の lammps_education_flow_win (https://github.com/by-student-2017/lammps_education_flow_win.git) から入力ファイルをダウンロードして解凍する。右側の[Clone or download]をクリックしていただくと Download ZIP が表示されます


□ シミュレーションの実行
1. 各種のフォルダの中にある run.bat をダブルクリックすれば計算が走る
2. cfg を Ovito で開けば構造が得られる
3. plot と記載のあるファイルをダブルクリックすれば図が得られる
  ※ 温度が目的の値になっているか、エネルギーが一定の値になっているかを確認してみてください
※ 以上の手順は、data.inにある原子の情報、そして、in.lmpのポテンシャルと出力の原子の情報を書きかえれば他の材料でも同様に計算が可能です（Avogadroなどのフリーソフトを用いて構造のファイル（data.in）を作られる方もいます）


□ tutorial_1_Fe_cyclohexane_Cr
  Fe/cyclohexane/Crの計算。


□ tutorial_2_Cu_toluene_Ni
  Cu/toluene/Niの計算。


□ tutorial_3_Co_toluene_Zr
  Cotoluene/Zr


□ tutorial_4_Ti_toluene_Mg
  Ti/toluene/Mgの計算。


□ tutorial_5_Al_DD_Ca
  Al/DD/Caの計算。


※ reaxffポテンシャルを使って、金属と有機物の界面を有する計算例を作ってみました。Mg, Al, Ca, Zrなどは活性が高すぎるため、酸化物や表面にOHなどを付けて表面を安定にした方が有機物が分解しなくてすみます。


※ Avogadro, VESTA, LibreOfficeを用いて構造を作っています。フリーソフトで初期構造（分子間の隙間を大きめに）を作って、構造緩和させたものをdata.inに入れています。


※ reaxffのファイルにreaxffポテンシャルをまとめておきました。Feが計算できるものはKISTにあるファイルではエラーが表示されたので私が修正しました（修正や誤っていたら申し訳ありません）。


※ これらの入力例は、とりあえず作ってみたという感じですので、より精度が高く、目的の構造を計算できるように入力ファイルを作って頂けましたら幸いに存じます。


------------------------------------------------------------------------------