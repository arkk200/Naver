<script lang="ts">
    const subNews = [
        "삼성SDS 낮아진 IT서비스 영업익, 기댈 것은 클라우드 뿐?",
        "‘에너지 효율’ 얼마나 좋아졌나… 2023년 삼성전자 에어컨·...",
        "OTT 불공정관행·단통법 추가지원금 상향에도 공정위 손댄다",
        "‘플랫폼’에 칼 겨눈 공정위, 올해 규율체계 마련",
        "[IT백과] ICT 국제표준을 만드는 이곳, 국제전기통신연합(I...",
        "[딜라이트닷넷] “세뱃돈으로 투자해볼까?” 부담 적고 흥미 ..."
    ]
</script>

<div class="sub-news">
    <div class="items">
        {#each subNews as news}
            <div>{news}</div>
        {/each}
    </div>
    <div class="footer">NNN 언론사에서 직접 편집한 뉴스입니다.</div>
</div>

<style lang="scss">
    .sub-news {
        font-size: 13px;
        color: var(--black01);
        height: 100%;

        .items {
            div {
                line-height: 26px;
            }
        }

        .footer {
            margin-top: 12px;
            color: var(--black04);
        }
    }
</style>