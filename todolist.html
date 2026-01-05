<!doctype html>
<html lang="ko">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Posture Coach</title>

  <style>
    :root{
      --bgA: #0ea5e9;
      --bgB: #a78bfa;
      --bgC: #22c55e;

      --card: rgba(255,255,255,.10);
      --card2: rgba(255,255,255,.14);
      --stroke: rgba(255,255,255,.22);
      --text: rgba(255,255,255,.92);
      --muted: rgba(255,255,255,.70);
      --shadow: 0 20px 60px rgba(0,0,0,.25);
    }

    body{
      margin:0;
      font-family: ui-sans-serif, system-ui, -apple-system, "Noto Sans KR", Segoe UI, Roboto, Arial, sans-serif;
      color: var(--text);
      min-height: 100svh;
      display:flex;
      align-items:center;
      justify-content:center;
      padding: 24px;
      transition: background 300ms ease;
      background:
        radial-gradient(1100px 700px at 12% 12%, rgba(255,255,255,.16), transparent 60%),
        radial-gradient(900px 600px at 88% 18%, rgba(255,255,255,.10), transparent 55%),
        linear-gradient(135deg, var(--bgA), var(--bgB) 55%, var(--bgC));
      overflow-x:hidden;
    }

    /* 상태별 배경 */
    body.state-good{
      background:
        radial-gradient(1100px 700px at 12% 12%, rgba(255,255,255,.20), transparent 60%),
        radial-gradient(900px 600px at 88% 18%, rgba(255,255,255,.12), transparent 55%),
        linear-gradient(135deg, #22c55e, #10b981 55%, #06b6d4);
    }
    body.state-bad{
      background:
        radial-gradient(1100px 700px at 12% 12%, rgba(255,255,255,.16), transparent 60%),
        radial-gradient(900px 600px at 88% 18%, rgba(255,255,255,.08), transparent 55%),
        linear-gradient(135deg, #ef4444, #f97316 55%, #f59e0b);
    }

    .wrap{ width:min(980px, 100%); }

    .topbar{
      display:flex;
      justify-content:space-between;
      align-items:flex-end;
      gap:12px;
      margin-bottom: 14px;
    }
    .title h1{
      margin:0;
      font-size:28px;
      letter-spacing:-0.5px;
      line-height:1.15;
    }
    .title p{
      margin:6px 0 0;
      font-size:13px;
      color: var(--muted);
    }

    .pill{
      border:1px solid var(--stroke);
      background: linear-gradient(180deg, rgba(255,255,255,.14), rgba(255,255,255,.06));
      backdrop-filter: blur(14px);
      border-radius:999px;
      padding:10px 12px;
      box-shadow: 0 10px 30px rgba(0,0,0,.18);
      font-size:12px;
      color: rgba(255,255,255,.88);
      white-space:nowrap;
    }

    .grid{
      display:grid;
      grid-template-columns: 1.2fr .8fr;
      gap:14px;
    }

    .card{
      border:1px solid var(--stroke);
      background: linear-gradient(180deg, var(--card2), var(--card));
      backdrop-filter: blur(18px);
      border-radius:18px;
      box-shadow: var(--shadow);
      padding:16px;
    }

    .controls{
      display:flex;
      gap:10px;
      align-items:center;
      justify-content:space-between;
      flex-wrap:wrap;
      margin-bottom: 12px;
    }

    .btn{
      border:none;
      outline:none;
      cursor:pointer;
      border-radius:14px;
      padding:12px 14px;
      color: rgba(255,255,255,.95);
      font-weight:700;
      font-size:14px;
      background: linear-gradient(135deg, rgba(255,255,255,.25), rgba(255,255,255,.08));
      border:1px solid rgba(255,255,255,.22);
      transition: transform .12s ease, filter .12s ease;
      box-shadow: 0 12px 30px rgba(0,0,0,.18);
      display:flex;
      align-items:center;
      gap:8px;
    }
    .btn:hover{ transform: translateY(-1px); filter:brightness(1.05); }
    .btn:active{ transform: translateY(0px); filter:brightness(.98); }

    .hint{
      display:flex;
      gap:8px;
      align-items:center;
      color: rgba(255,255,255,.72);
      font-size:12px;
    }
    .dot{
      width:10px; height:10px; border-radius:999px;
      background: rgba(255,255,255,.55);
      box-shadow: 0 0 0 4px rgba(255,255,255,.08);
    }

    .camWrap{
      display:flex;
      gap:14px;
      align-items:stretch;
      flex-wrap:wrap;
    }

    canvas{
      width: 320px;
      height: 320px;
      border-radius:16px;
      border:1px solid rgba(255,255,255,.20);
      background: rgba(0,0,0,.16);
      box-shadow: 0 14px 40px rgba(0,0,0,.22);
    }

    .statusBox{
      flex:1;
      min-width: 240px;
      display:flex;
      flex-direction:column;
      gap:12px;
      justify-content:space-between;
    }

    .statusTop{
      display:flex;
      align-items:center;
      justify-content:space-between;
      gap:12px;
    }

    .badge{
      padding:8px 10px;
      border-radius:999px;
      border:1px solid rgba(255,255,255,.22);
      background: rgba(0,0,0,.14);
      font-size:12px;
      color: rgba(255,255,255,.86);
    }

    .big{
      font-size:20px;
      font-weight:800;
      letter-spacing:-0.2px;
    }
    .sub{
      margin-top:4px;
      font-size:12px;
      color: rgba(255,255,255,.70);
      line-height:1.4;
    }

    .meter{
      border:1px solid rgba(255,255,255,.18);
      background: rgba(0,0,0,.14);
      border-radius:14px;
      padding:12px;
    }

    .barRow{
      display:flex;
      justify-content:space-between;
      font-size:12px;
      color: rgba(255,255,255,.80);
      margin-bottom:8px;
    }

    .bar{
      height: 10px;
      border-radius:999px;
      background: rgba(255,255,255,.16);
      overflow:hidden;
      border: 1px solid rgba(255,255,255,.14);
    }
    .fill{
      height:100%;
      width:0%;
      border-radius:999px;
      background: rgba(255,255,255,.70);
      transition: width 180ms ease;
    }

    .labels{
      display:flex;
      flex-direction:column;
      gap:8px;
      margin-top:12px;
    }
    .labelItem{
      display:flex;
      align-items:center;
      justify-content:space-between;
      gap:10px;
      padding:10px 12px;
      border-radius:14px;
      border:1px solid rgba(255,255,255,.18);
      background: rgba(0,0,0,.10);
      font-size:13px;
      color: rgba(255,255,255,.88);
    }
    .labelItem span:last-child{
      color: rgba(255,255,255,.75);
      font-variant-numeric: tabular-nums;
    }

    .sideTitle{
      display:flex;
      align-items:center;
      justify-content:space-between;
      gap:10px;
      margin-bottom:10px;
    }
    .sideTitle h2{
      margin:0;
      font-size:16px;
      letter-spacing:-0.2px;
    }
    .small{
      font-size:12px;
      color: rgba(255,255,255,.70);
    }

    @media (max-width: 900px){
      .grid{ grid-template-columns: 1fr; }
      canvas{ width:100%; height:auto; aspect-ratio:1/1; }
    }
  </style>
</head>

<body>
  <div class="wrap">
    <div class="topbar">
      <div class="title">
        <h1>Posture Coach</h1>
        <p>자세를 인식하고, <b>바른 자세 50%↑</b>면 상쾌한 배경 / <b>안좋은 자세 50%↑</b>면 경고 배경으로 바뀝니다.</p>
      </div>
      <div class="pill" id="pillText">대기 중</div>
    </div>

    <div class="grid">
      <!-- Left: Camera + Live status -->
      <div class="card">
        <div class="controls">
          <button class="btn" type="button" id="startBtn">
            <!-- play icon -->
            <svg width="18" height="18" viewBox="0 0 24 24" fill="none" aria-hidden="true">
              <path d="M8 5v14l11-7-11-7Z" stroke="white" stroke-width="2" stroke-linejoin="round"/>
            </svg>
            Start
          </button>

          <div class="hint">
            <span class="dot" id="liveDot"></span>
            <span id="liveText">웹캠이 시작되면 자동으로 분석합니다</span>
          </div>
        </div>

        <div class="camWrap">
          <canvas id="canvas"></canvas>

          <div class="statusBox">
            <div class="statusTop">
              <div>
                <div class="big" id="statusTitle">Ready</div>
                <div class="sub" id="statusSub">Start를 누르면 웹캠 권한을 요청해요.</div>
              </div>
              <div class="badge" id="statusBadge">—</div>
            </div>

            <div class="meter">
              <div class="barRow">
                <span>바른 자세</span>
                <span id="goodPct">0%</span>
              </div>
              <div class="bar"><div class="fill" id="goodBar"></div></div>

              <div style="height:10px"></div>

              <div class="barRow">
                <span>안좋은 자세</span>
                <span id="badPct">0%</span>
              </div>
              <div class="bar"><div class="fill" id="badBar"></div></div>

              <div class="sub" style="margin-top:10px">
                기준: 둘 중 하나가 <b>50%</b>를 넘으면 해당 상태로 배경이 바뀝니다.
              </div>
            </div>
          </div>
        </div>
      </div>

      <!-- Right: Raw predictions -->
      <div class="card">
        <div class="sideTitle">
          <h2>모델 결과</h2>
          <div class="small">Raw probabilities</div>
        </div>
        <div id="label-container" class="labels"></div>
      </div>
    </div>
  </div>

  <script src="https://cdn.jsdelivr.net/npm/@tensorflow/tfjs@1.3.1/dist/tf.min.js"></script>
  <script src="https://cdn.jsdelivr.net/npm/@teachablemachine/pose@0.8/dist/teachablemachine-pose.min.js"></script>

  <script>
    // ✅ 모델 경로
    const URL = "./my_model/";

    // ✅ 여기 2개를 "네 모델 클래스 이름"으로 꼭 맞춰줘!
    // 예: Teachable Machine에서 className이 "good_posture", "bad_posture" 이런 식이면 그대로 적기
    const GOOD_LABEL = "바른자세";   // <-- 수정 필요할 수 있음
    const BAD_LABEL  = "안좋은자세"; // <-- 수정 필요할 수 있음

    // 상태
    let model, webcam, ctx, maxPredictions;
    let labelContainer;

    // UI refs
    const startBtn = document.getElementById("startBtn");
    const pillText = document.getElementById("pillText");
    const liveDot = document.getElementById("liveDot");
    const liveText = document.getElementById("liveText");

    const statusTitle = document.getElementById("statusTitle");
    const statusSub = document.getElementById("statusSub");
    const statusBadge = document.getElementById("statusBadge");

    const goodPctEl = document.getElementById("goodPct");
    const badPctEl  = document.getElementById("badPct");
    const goodBar   = document.getElementById("goodBar");
    const badBar    = document.getElementById("badBar");

    startBtn.addEventListener("click", init);

    function setState(type){
      document.body.classList.remove("state-good","state-bad");
      if(type === "good") document.body.classList.add("state-good");
      if(type === "bad")  document.body.classList.add("state-bad");
    }

    function fmtPct(x){
      return Math.round(x * 100);
    }

    async function init() {
      try{
        pillText.textContent = "모델 로딩 중…";
        statusTitle.textContent = "Loading…";
        statusSub.textContent = "모델과 메타데이터를 불러오는 중입니다.";
        liveDot.style.background = "rgba(255,255,255,.55)";
        liveText.textContent = "권한 요청이 뜨면 허용을 눌러주세요.";

        const modelURL = URL + "model.json";
        const metadataURL = URL + "metadata.json";

        model = await tmPose.load(modelURL, metadataURL);
        maxPredictions = model.getTotalClasses();

        // webcam setup
        const size = 320; // 더 예쁘게 크게
        const flip = true;
        webcam = new tmPose.Webcam(size, size, flip);
        await webcam.setup();
        await webcam.play();
        window.requestAnimationFrame(loop);

        // canvas
        const canvas = document.getElementById("canvas");
        canvas.width = size;
        canvas.height = size;
        ctx = canvas.getContext("2d");

        // labels container
        labelContainer = document.getElementById("label-container");
        labelContainer.innerHTML = "";
        for (let i = 0; i < maxPredictions; i++) {
          const row = document.createElement("div");
          row.className = "labelItem";
          row.innerHTML = `<span>—</span><span>0%</span>`;
          labelContainer.appendChild(row);
        }

        pillText.textContent = "라이브 분석 중";
        statusTitle.textContent = "Analyzing";
        statusSub.textContent = "지금 자세를 인식하고 있어요.";
        statusBadge.textContent = "LIVE";
        liveDot.style.background = "rgba(255,255,255,.85)";
        liveText.textContent = "웹캠이 켜졌어요. 바른 자세를 유지해보세요!";
      }catch(err){
        console.error(err);
        pillText.textContent = "에러";
        statusTitle.textContent = "Error";
        statusSub.textContent = "웹캠 권한 또는 모델 경로(URL)를 확인해주세요.";
        statusBadge.textContent = "FAILED";
        liveText.textContent = "오류가 발생했어요. 콘솔을 확인해 주세요.";
      }
    }

    async function loop(timestamp) {
      webcam.update();
      await predict();
      window.requestAnimationFrame(loop);
    }

    async function predict() {
      const { pose, posenetOutput } = await model.estimatePose(webcam.canvas);
      const prediction = await model.predict(posenetOutput);

      // label UI 업데이트 + good/bad 확률 찾기
      let goodProb = 0;
      let badProb = 0;

      for (let i = 0; i < maxPredictions; i++) {
        const name = prediction[i].className;
        const prob = prediction[i].probability;

        // 오른쪽 raw 리스트 업데이트
        const row = labelContainer.childNodes[i];
        row.firstChild.textContent = name;
        row.lastChild.textContent = `${fmtPct(prob)}%`;

        // good/bad 추적
        if(name === GOOD_LABEL) goodProb = prob;
        if(name === BAD_LABEL)  badProb  = prob;
      }

      // 프로그레스 바 + 퍼센트
      goodPctEl.textContent = `${fmtPct(goodProb)}%`;
      badPctEl.textContent  = `${fmtPct(badProb)}%`;
      goodBar.style.width = `${fmtPct(goodProb)}%`;
      badBar.style.width  = `${fmtPct(badProb)}%`;

      // ✅ 50% 기준으로 배경/상태 변경
      if(goodProb > 0.5 && goodProb >= badProb){
        setState("good");
        statusTitle.textContent = "바른 자세 👍";
        statusSub.textContent = "좋아요! 허리/목 라인 유지 중.";
        statusBadge.textContent = "GOOD";
        pillText.textContent = `바른 자세 ${fmtPct(goodProb)}%`;
      } else if(badProb > 0.5 && badProb > goodProb){
        setState("bad");
        statusTitle.textContent = "자세 경고 ⚠️";
        statusSub.textContent = "고개/어깨 정렬을 다시 맞춰보세요.";
        statusBadge.textContent = "WARNING";
        pillText.textContent = `안좋은 자세 ${fmtPct(badProb)}%`;
      } else {
        setState(null);
        statusTitle.textContent = "측정 중…";
        statusSub.textContent = "조금 더 안정적으로 자세를 잡아주세요.";
        statusBadge.textContent = "NEUTRAL";
        pillText.textContent = "중립 상태";
      }

      // 포즈 그리기
      drawPose(pose);
    }

    function drawPose(pose) {
      if (webcam.canvas) {
        ctx.drawImage(webcam.canvas, 0, 0);

        if (pose) {
          const minPartConfidence = 0.5;
          tmPose.drawKeypoints(pose.keypoints, minPartConfidence, ctx);
          tmPose.drawSkeleton(pose.keypoints, minPartConfidence, ctx);
        }
      }
    }
  </script>
</body>
</html>
