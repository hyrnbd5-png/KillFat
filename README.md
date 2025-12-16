<!doctype html>
<html lang="ko">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <meta name="description" content="항비만 유산균 FatSlim(HY7601+KY1032) – 박람회/광고용 제품 소개 페이지" />
  <title>FatSlim | HY7601 + KY1032</title>

  <style>
    :root{
      --bg:#0b0f17;
      --panel:#101826;
      --panel2:#0f1522;
      --text:#eaf0ff;
      --muted:#a9b4d0;
      --line:rgba(255,255,255,.10);
      --accent:#7c5cff;
      --accent2:#26d3ff;
      --ok:#33e6a6;
      --warn:#ffd166;
      --shadow: 0 20px 60px rgba(0,0,0,.45);
      --radius: 18px;
      --radius2: 26px;
      --max: 1100px;
    }
    *{box-sizing:border-box}
    body{
      margin:0;
      font-family: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, "Noto Sans KR", "Apple SD Gothic Neo", sans-serif;
      color:var(--text);
      background:
        radial-gradient(1200px 700px at 20% 0%, rgba(124,92,255,.25), transparent 60%),
        radial-gradient(900px 600px at 90% 10%, rgba(38,211,255,.18), transparent 55%),
        radial-gradient(800px 600px at 50% 120%, rgba(51,230,166,.12), transparent 60%),
        var(--bg);
      line-height:1.55;
    }
    a{color:inherit}
    .wrap{max-width:var(--max); margin:0 auto; padding:28px 18px 70px}
    header{
      display:flex; align-items:center; justify-content:space-between;
      gap:14px; padding:8px 2px 18px;
    }
    .brand{
      display:flex; align-items:center; gap:10px; text-decoration:none;
    }
    .logo{
      width:36px; height:36px; border-radius:12px;
      background: linear-gradient(135deg, var(--accent), var(--accent2));
      box-shadow: 0 10px 30px rgba(124,92,255,.25);
    }
    .brand b{letter-spacing:.2px}
    nav{display:flex; gap:10px; flex-wrap:wrap; justify-content:flex-end}
    .pill{
      border:1px solid var(--line);
      background:rgba(255,255,255,.04);
      padding:9px 12px; border-radius:999px;
      text-decoration:none; color:var(--muted);
      font-size:13px;
      transition:transform .15s ease, background .15s ease;
    }
    .pill:hover{transform:translateY(-1px); background:rgba(255,255,255,.07); color:var(--text)}
    .hero{
      margin-top:10px;
      background: linear-gradient(180deg, rgba(255,255,255,.06), rgba(255,255,255,.02));
      border:1px solid var(--line);
      border-radius: var(--radius2);
      padding: 34px 22px;
      box-shadow: var(--shadow);
      position:relative;
      overflow:hidden;
    }
    .hero:before{
      content:"";
      position:absolute; inset:-200px -200px auto auto;
      width:420px; height:420px;
      background: radial-gradient(circle at 30% 30%, rgba(124,92,255,.35), transparent 60%);
      filter: blur(6px);
    }
    .grid-hero{
      display:grid;
      grid-template-columns: 1.25fr .9fr;
      gap:22px;
      align-items:center;
    }
    @media (max-width: 900px){
      .grid-hero{grid-template-columns:1fr}
    }
    .badgeRow{display:flex; gap:10px; flex-wrap:wrap; margin-bottom:14px}
    .badge{
      font-size:12px;
      color:var(--muted);
      border:1px solid var(--line);
      background:rgba(255,255,255,.04);
      padding:7px 10px;
      border-radius:999px;
    }
    h1{
      margin:0 0 10px;
      font-size: clamp(30px, 4.2vw, 54px);
      letter-spacing:-.6px;
      line-height:1.08;
    }
    .sub{
      margin:0 0 16px;
      color:var(--muted);
      font-size: 16px;
      max-width: 60ch;
    }
    .ctaRow{display:flex; gap:12px; flex-wrap:wrap; align-items:center; margin-top:16px}
    .btn{
      display:inline-flex; align-items:center; justify-content:center; gap:10px;
      padding: 12px 14px;
      border-radius: 14px;
      border:1px solid var(--line);
      background: rgba(255,255,255,.06);
      text-decoration:none;
      color:var(--text);
      font-weight:650;
      box-shadow: 0 14px 40px rgba(0,0,0,.35);
      transition: transform .16s ease, background .16s ease;
      cursor:pointer;
    }
    .btn:hover{transform: translateY(-1px); background: rgba(255,255,255,.09)}
    .btn.primary{
      border: 0;
      background: linear-gradient(135deg, var(--accent), var(--accent2));
      color:#07101b;
    }
    .btn.primary:hover{filter:brightness(1.03)}
    .hint{font-size:12px; color:var(--muted)}
    .panel{
      margin-top:18px;
      display:grid;
      grid-template-columns: repeat(3, 1fr);
      gap:12px;
    }
    @media (max-width: 900px){ .panel{grid-template-columns:1fr} }
    .card{
      border:1px solid var(--line);
      background: rgba(255,255,255,.03);
      border-radius: var(--radius);
      padding: 16px;
    }
    .kpi{
      display:flex; align-items:flex-start; justify-content:space-between; gap:10px;
    }
    .kpi b{font-size:26px}
    .kpi span{color:var(--muted); font-size:13px}
    .tag{
      font-size:12px;
      color:#07101b;
      background: rgba(51,230,166,.92);
      padding: 6px 10px;
      border-radius: 999px;
      font-weight:700;
      white-space:nowrap;
    }
    .tag.warn{background: rgba(255,209,102,.92)}
    .section{margin-top:26px}
    .section h2{
      margin:0 0 10px;
      font-size: 22px;
      letter-spacing:-.3px;
    }
    .section p{margin:0 0 12px; color:var(--muted)}
    .two{
      display:grid;
      grid-template-columns: 1fr 1fr;
      gap:12px;
    }
    @media (max-width: 900px){ .two{grid-template-columns:1fr} }
    .list{
      margin:0; padding-left:18px; color:var(--muted);
    }
    .list li{margin:8px 0}
    .quoteGrid{
      display:grid;
      grid-template-columns: repeat(3, 1fr);
      gap:12px;
      margin-top:12px;
    }
    @media (max-width: 900px){ .quoteGrid{grid-template-columns:1fr} }
    .quote{
      border:1px solid var(--line);
      background: linear-gradient(180deg, rgba(255,255,255,.05), rgba(255,255,255,.02));
      border-radius: var(--radius);
      padding: 16px;
    }
    .quote .meta{margin-top:10px; font-size:12px; color:var(--muted)}
    .hr{height:1px; background:var(--line); margin:16px 0}
    details{
      border:1px solid var(--line);
      border-radius: var(--radius);
      padding: 12px 14px;
      background: rgba(255,255,255,.03);
    }
    details + details{margin-top:10px}
    summary{cursor:pointer; font-weight:650}
    summary::marker{color:var(--muted)}
    .foot{
      margin-top:26px;
      color:var(--muted);
      font-size:12px;
    }
    .qrBox{
      display:flex; gap:14px; align-items:center; flex-wrap:wrap;
    }
    .qr{
      width:120px; height:120px; border-radius: 18px;
      border:1px dashed rgba(255,255,255,.25);
      display:flex; align-items:center; justify-content:center;
      color:rgba(255,255,255,.6);
      background: rgba(255,255,255,.02);
    }
    .mini{
      font-size:12px; color:var(--muted)
    }
    .accentLine{
      height:2px; width:92px; border-radius: 99px;
      background: linear-gradient(90deg, var(--accent), var(--accent2));
      margin:10px 0 14px;
    }
    .fineprint{
      font-size:11px;
      color:rgba(233,241,255,.62);
      border:1px solid rgba(255,255,255,.10);
      background: rgba(0,0,0,.16);
      padding: 12px 14px;
      border-radius: 16px;
    }
    .mutedLink{color:var(--muted); text-decoration:underline dotted; text-underline-offset:3px}
  </style>
</head>

<body>
  <div class="wrap">
    <header>
      <a class="brand" href="#top" aria-label="FatSlim Home">
        <span class="logo" aria-hidden="true"></span>
        <div>
          <b>FatSlim</b><div class="hint">HY7601 + KY1032</div>
        </div>
      </a>
      <nav aria-label="Page">
        <a class="pill" href="#why">제품 포인트</a>
        <a class="pill" href="#formula">균주/포뮬러</a>
        <a class="pill" href="#expo">박람회 안내</a>
        <a class="pill" href="#faq">FAQ</a>
      </nav>
    </header>

    <main id="top" class="hero">
      <div class="grid-hero">
        <div>
          <div class="badgeRow">
            <span class="badge">항비만 유산균 컨셉</span>
            <span class="badge">박람회·광고용 랜딩</span>
            <span class="badge">간결한 원페이지</span>
          </div>

          <h1>가벼운 루틴을 위한<br/>프로바이오틱스 솔루션</h1>
          <p class="sub">
            <b>FatSlim</b>은 <b>HY7601 + KY1032</b> 균주 조합을 중심으로,
            일상에서 ‘체지방 관리 루틴’에 자연스럽게 녹아드는 제품 경험을 지향합니다.
          </p>

          <div class="ctaRow">
            <!-- 박람회에서 가장 많이 쓰는 동선: "상담/샘플/카탈로그" -->
            <a class="btn primary" href="#expo">부스 상담/샘플 요청</a>
            <a class="btn" href="#catalog">제품 브로슈어 보기</a>
            <span class="hint">※ 문구/수치/근거는 최종 심의/내부 자료에 맞춰 업데이트 권장</span>
          </div>

          <div class="panel" style="margin-top:18px">
            <div class="card">
              <div class="kpi">
                <div>
                  <b>2-스트레인</b><br/>
                  <span>HY7601 + KY1032</span>
                </div>
                <span class="tag">COMBO</span>
              </div>
              <div class="hr"></div>
              <div class="hint">핵심 메시지: “조합 기반 설계”</div>
            </div>

            <div class="card">
              <div class="kpi">
                <div>
                  <b>데일리</b><br/>
                  <span>루틴형 섭취 컨셉</span>
                </div>
                <span class="tag warn">DAILY</span>
              </div>
              <div class="hr"></div>
              <div class="hint">박람회/광고에서 이해가 빠른 구조</div>
            </div>

            <div class="card">
              <div class="kpi">
                <div>
                  <b>클린</b><br/>
                  <span>심플한 정보 설계</span>
                </div>
                <span class="tag" style="background:rgba(38,211,255,.92)">CLEAR</span>
              </div>
              <div class="hr"></div>
              <div class="hint">원페이지로 핵심만 전달</div>
            </div>
          </div>
        </div>

        <!-- 우측 비주얼(제품 이미지) -->
        <div class="card" style="background:rgba(255,255,255,.02)">
          <h2 style="margin:0 0 10px; font-size:18px">제품 이미지 영역</h2>
          <div class="hint" style="margin-bottom:10px">
            아래 박스에 제품 컷(정면 PNG/JPG)을 넣으면 완성도가 급상승해요.
          </div>

          <!-- 이미지 교체: src를 실제 파일 경로로 변경 -->
          <div style="border:1px dashed rgba(255,255,255,.22); border-radius:18px; padding:14px; text-align:center">
            <img
              src="assets/fatslim-product.png"
              alt="FatSlim 제품 이미지"
              style="max-width:100%; height:auto; border-radius:14px; display:block; margin:0 auto"
              onerror="this.style.display='none'; this.nextElementSibling.style.display='block';"
            />
            <div style="display:none; color:rgba(255,255,255,.6); padding:42px 10px">
              assets/fatslim-product.png<br/>파일을 추가하면 여기 표시됩니다.
            </div>
          </div>

          <div class="hr"></div>
          <div class="mini">
            TIP: 박람회용이면 배경이 투명한 PNG(정면 컷) + 1:1 썸네일을 같이 준비하는 것을 추천.
          </div>
        </div>
      </div>
    </main>

    <section id="why" class="section">
      <h2>왜 FatSlim인가</h2>
      <div class="accentLine"></div>
      <p>
        박람회/광고 랜딩은 “설명”보다 “이해”가 먼저라서, 메시지를 3~5개의 포인트로 압축하는 것이 효율적입니다.
        아래 구성은 참고 페이지와 동일한 ‘카드형 핵심 가치 전달’ 패턴을 따릅니다. :contentReference[oaicite:1]{index=1}
      </p>

      <div class="two">
        <div class="card">
          <h3 style="margin:0 0 8px; font-size:16px">1) 체지방 관리 루틴에 초점</h3>
          <ul class="list">
            <li>일상 속 섭취 루틴과 결합하기 쉬운 메시지 설계</li>
            <li>“바로 이해되는” 단문형 카피로 부스/광고 매체에 적합</li>
          </ul>
        </div>
        <div class="card">
          <h3 style="margin:0 0 8px; font-size:16px">2) 2-스트레인 조합 컨셉</h3>
          <ul class="list">
            <li>HY7601 + KY1032 조합을 핵심 자산으로 고정</li>
            <li>세부 근거(시험 설계/데이터)는 ‘브로슈어’로 분리 가능</li>
          </ul>
        </div>
      </div>

      <div class="quoteGrid" aria-label="Testimonials">
        <div class="quote">
          <div style="font-weight:700; font-size:14px">“부스에서 설명이 빨라요.”</div>
          <div class="meta">관람객 피드백 예시 • 체험/상담</div>
          <div class="hint" style="margin-top:10px">※ 실제 후기/수치는 내부 자료로 교체 권장</div>
        </div>
        <div class="quote">
          <div style="font-weight:700; font-size:14px">“핵심만 보여줘서 기억에 남아요.”</div>
          <div class="meta">광고 랜딩 예시 • 요약형 구조</div>
          <div class="hint" style="margin-top:10px">※ 플랫폼 정책/표현 규정 준수 필요</div>
        </div>
        <div class="quote">
          <div style="font-weight:700; font-size:14px">“브로슈어로 이어지니 설득이 쉬워요.”</div>
          <div class="meta">영업/파트너 예시 • 자료 연동</div>
          <div class="hint" style="margin-top:10px">※ QR/카탈로그 링크 연결 추천</div>
        </div>
      </div>
    </section>

    <section id="formula" class="section">
      <h2>균주/포뮬러 한눈에 보기</h2>
      <div class="accentLine"></div>
      <p>
        이 섹션은 “전문성”을 보여주되, 과도한 의학적 단정 표현은 피하는 방향으로 설계했습니다.
        (최종 문구는 제품 표시·광고 심의/내부 근거자료에 맞춰 조정 권장)
      </p>

      <div class="two">
        <div class="card">
          <h3 style="margin:0 0 8px; font-size:16px">핵심 구성</h3>
          <ul class="list">
            <li><b>HY7601</b> (균주 정보/유래/특징: 내부자료로 기입)</li>
            <li><b>KY1032</b> (균주 정보/유래/특징: 내부자료로 기입)</li>
            <li>섭취 방법: 1일 1회 / 식전·식후 등 (권장 섭취 가이드로 교체)</li>
          </ul>
        </div>
        <div class="card">
          <h3 style="margin:0 0 8px; font-size:16px">박람회용 전달 포인트</h3>
          <ul class="list">
            <li>“2-스트레인 조합” → 차별점 한 문장으로 고정</li>
            <li>디테일 데이터는 브로슈어(PDF)로 분리해 QR 연결</li>
            <li>문의/샘플/대리점 제안 CTA를 상단에 반복 배치</li>
          </ul>
        </div>
      </div>

      <div class="fineprint" style="margin-top:12px">
        <b>고지 문구(예시)</b><br/>
        본 페이지는 정보 제공을 목적으로 하며, 개인에 따라 체감 결과는 다를 수 있습니다.
        본 제품은 의약품이 아니며 질병의 예방·치료를 위한 목적이 아닙니다.
      </div>
    </section>

    <section id="catalog" class="section">
      <h2>카탈로그/근거자료 연결</h2>
      <div class="accentLine"></div>
      <p>
        박람회 현장에서는 “설명 → QR → 자료 확인” 동선이 가장 전환이 잘 나옵니다.
        아래 버튼을 실제 PDF/노션/구글드라이브 링크로 바꾸면 됩니다.
      </p>
      <div class="ctaRow">
        <a class="btn" href="#" onclick="alert('여기에 PDF 링크를 연결하세요. 예: assets/fatslim-brochure.pdf'); return false;">브로슈어(PDF) 열기</a>
        <a class="btn" href="#" onclick="alert('여기에 시험/원료/인증 자료 링크를 연결하세요.'); return false;">근거자료 보기</a>
      </div>
      <div class="hint" style="margin-top:10px">
        TIP: PDF를 저장소에 올리면 GitHub Pages에서 그대로 배포 가능합니다(정적 파일 호스팅). :contentReference[oaicite:2]{index=2}
      </div>
    </section>

    <section id="expo" class="section">
      <h2>박람회 상담/샘플 요청</h2>
      <div class="accentLine"></div>
      <p>
        아래 영역은 부스 스탭이 태블릿으로 띄워두거나, 광고 랜딩의 최종 CTA로 사용하기 좋습니다.
        “연락처 수집”은 보통 외부 폼(구글폼/폼스프리 등)과 연동합니다.
      </p>

      <div class="card">
        <div class="qrBox">
          <div class="qr" aria-label="QR placeholder">QR</div>
          <div>
            <div style="font-weight:750; font-size:16px">QR로 상담 신청</div>
            <div class="mini">QR 이미지를 생성해 `assets/qr.png`로 넣고, 아래 img 태그 src를 바꾸세요.</div>
            <div class="hr"></div>

            <!-- QR 이미지 교체 -->
            <img
              src="assets/qr.png"
              alt="상담 신청 QR"
              style="max-width:160px; height:auto; border-radius:14px; display:block"
              onerror="this.style.display='none';"
            />

            <div class="ctaRow" style="margin-top:12px">
              <!-- 실제 문의 메일/전화/카카오 채널로 변경 -->
              <a class="btn primary" href="mailto:hello@example.com?subject=FatSlim%20%EB%B0%95%EB%9E%8C%ED%9A%8C%20%EC%83%81%EB%8B%B4%20%EC%9A%94%EC%B2%AD">이메일 문의</a>
              <a class="btn" href="tel:+82-10-0000-0000">전화 연결</a>
              <a class="btn" href="#" onclick="alert('카카오채널/폼 링크로 교체하세요.'); return false;">상담 폼 열기</a>
            </div>

            <div class="hint" style="margin-top:10px">
              현장용 추천: “담당자/회사/연락처/관심(샘플·대리점·OEM)” 4필드 정도가 전환율이 좋습니다.
            </div>
          </div>
        </div>
      </div>
    </section>

    <section id="faq" class="section">
      <h2>FAQ</h2>
      <div class="accentLine"></div>

      <details>
        <summary>Q. HY7601 + KY1032는 어떤 포지셔닝인가요?</summary>
        <div class="hint" style="margin-top:10px">
          A. “2-스트레인 조합 기반 체지방 관리 루틴”으로 간단히 정의하고,
          세부 근거(시험 설계/데이터/섭취 가이드)는 브로슈어로 분리해 전달하는 방식을 권장합니다.
        </div>
      </details>

      <details>
        <summary>Q. 박람회에서 가장 효과적인 CTA는 무엇인가요?</summary>
        <div class="hint" style="margin-top:10px">
          A. (1) 샘플 요청, (2) 대리점/파트너 상담, (3) 카탈로그 다운로드 3가지를 상단/하단에 반복 배치하는 구성이 일반적으로 효율적입니다.
        </div>
      </details>

      <details>
        <summary>Q. 표현 수위(효능/효과)는 어디까지 가능한가요?</summary>
        <div class="hint" style="margin-top:10px">
          A. 최종 광고 문구는 반드시 제품 유형/표시 기준/심의 기준 및 보유 근거자료에 맞춰 조정해야 합니다.
          본 템플릿은 과도한 단정 표현을 피하도록 작성되었습니다.
        </div>
      </details>
    </section>

    <footer class="foot">
      <div class="fineprint">
        <b>Disclaimer</b><br/>
        본 페이지는 박람회/광고용 제품 소개 자료(초안)입니다. 실제 판매/광고 집행 전,
        관련 법령 및 플랫폼 정책, 내부 근거자료와의 정합성 검토를 권장합니다.
      </div>
      <div style="margin-top:10px">
        © <span id="y"></span> FatSlim. All rights reserved.
      </div>
    </footer>
  </div>

  <script>
    document.getElementById("y").textContent = new Date().getFullYear();
  </script>
</body>
</html>
