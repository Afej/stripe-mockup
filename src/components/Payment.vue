<template>
  <tr>
    <td class="checkbox-icon">
      <svg
        width="24"
        height="24"
        viewBox="0 0 24 24"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <g filter="url(#filter0_ddd)">
          <rect x="5" y="3" width="14" height="14" rx="4" fill="white" />
        </g>
        <defs>
          <filter
            id="filter0_ddd"
            x="0"
            y="0"
            width="24"
            height="24"
            filterUnits="userSpaceOnUse"
            color-interpolation-filters="sRGB"
          >
            <feFlood flood-opacity="0" result="BackgroundImageFix" />
            <feColorMatrix
              in="SourceAlpha"
              type="matrix"
              values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
              result="hardAlpha"
            />
            <feOffset dy="1" />
            <feGaussianBlur stdDeviation="0.5" />
            <feColorMatrix
              type="matrix"
              values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.12 0"
            />
            <feBlend
              mode="normal"
              in2="BackgroundImageFix"
              result="effect1_dropShadow"
            />
            <feColorMatrix
              in="SourceAlpha"
              type="matrix"
              values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
              result="hardAlpha"
            />
            <feMorphology
              radius="1"
              operator="dilate"
              in="SourceAlpha"
              result="effect2_dropShadow"
            />
            <feOffset />
            <feColorMatrix
              type="matrix"
              values="0 0 0 0 0.235294 0 0 0 0 0.258824 0 0 0 0 0.341176 0 0 0 0.16 0"
            />
            <feBlend
              mode="normal"
              in2="effect1_dropShadow"
              result="effect2_dropShadow"
            />
            <feColorMatrix
              in="SourceAlpha"
              type="matrix"
              values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
              result="hardAlpha"
            />
            <feOffset dy="2" />
            <feGaussianBlur stdDeviation="2.5" />
            <feColorMatrix
              type="matrix"
              values="0 0 0 0 0.235294 0 0 0 0 0.258824 0 0 0 0 0.341176 0 0 0 0.08 0"
            />
            <feBlend
              mode="normal"
              in2="effect2_dropShadow"
              result="effect3_dropShadow"
            />
            <feBlend
              mode="normal"
              in="SourceGraphic"
              in2="effect3_dropShadow"
              result="shape"
            />
          </filter>
        </defs>
      </svg>
    </td>
    <td class="amount">{{ payment.amount }}</td>
    <td class="description">
      <span class="label-btn">
        {{ payment.description.label }}
        <svg
          width="16"
          height="16"
          viewBox="0 0 16 16"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            fill-rule="evenodd"
            clip-rule="evenodd"
            d="M5.97274 11.9097L2.21974 8.19125C1.92724 7.89575 1.92724 7.4165 2.21974 7.12175C2.51224 6.827 2.98774 6.82625 3.28024 7.12175L6.50074 10.2897L12.7167 4.09625C13.0092 3.8015 13.4847 3.8015 13.7772 4.09625C14.0697 4.391 14.0697 4.871 13.7772 5.16575L7.02499 11.906C6.88579 12.0455 6.69705 12.1241 6.50001 12.1248C6.30298 12.1255 6.11368 12.0482 5.97349 11.9097H5.97274Z"
            fill="#0E6245"
          />
        </svg>
      </span>
      {{ payment.description.text }}
    </td>
    <td class="customer">{{ payment.customer }}</td>
    <td class="date">{{ payment.date }}</td>
    <td class="more-icon">
      <svg
        width="12"
        height="4"
        viewBox="0 0 12 4"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          fill-rule="evenodd"
          clip-rule="evenodd"
          d="M1.5 3.5C1.10218 3.5 0.720644 3.34196 0.43934 3.06066C0.158035 2.77936 0 2.39782 0 2C0 1.60218 0.158035 1.22064 0.43934 0.93934C0.720644 0.658035 1.10218 0.5 1.5 0.5C1.89782 0.5 2.27936 0.658035 2.56066 0.93934C2.84196 1.22064 3 1.60218 3 2C3 2.39782 2.84196 2.77936 2.56066 3.06066C2.27936 3.34196 1.89782 3.5 1.5 3.5ZM6 3.5C5.60218 3.5 5.22064 3.34196 4.93934 3.06066C4.65804 2.77936 4.5 2.39782 4.5 2C4.5 1.60218 4.65804 1.22064 4.93934 0.93934C5.22064 0.658035 5.60218 0.5 6 0.5C6.39782 0.5 6.77936 0.658035 7.06066 0.93934C7.34196 1.22064 7.5 1.60218 7.5 2C7.5 2.39782 7.34196 2.77936 7.06066 3.06066C6.77936 3.34196 6.39782 3.5 6 3.5ZM10.5 3.5C10.1022 3.5 9.72064 3.34196 9.43934 3.06066C9.15804 2.77936 9 2.39782 9 2C9 1.60218 9.15804 1.22064 9.43934 0.93934C9.72064 0.658035 10.1022 0.5 10.5 0.5C10.8978 0.5 11.2794 0.658035 11.5607 0.93934C11.842 1.22064 12 1.60218 12 2C12 2.39782 11.842 2.77936 11.5607 3.06066C11.2794 3.34196 10.8978 3.5 10.5 3.5Z"
          fill="#4F566B"
        />
      </svg>
    </td>
  </tr>
</template>

<script>
export default {
  name: "Payment",
  props: {
    payment: Object,
  },
};
</script>

<style scoped>
td {
  padding: 10px 0;
  border-bottom: 1px solid #e3e8ee;
}

.amount {
  font-style: normal;
  font-weight: 600;
  font-size: 14px;
  line-height: 17px;
  color: #1a1f36;
}

.description {
  font-size: 13px;
  line-height: 16px;
  color: #4f566b;
}

.label-btn {
  width: 93px;
  margin-right: 16px;
  padding: 3px 4px 3px 6px;
  background: #cbf4c9;
  border-radius: 4px;
  font-style: normal;
  font-weight: 500;
  font-size: 12px;
  line-height: 14px;
  color: #0e6245;
}

.label-btn svg {
  padding-top: 5px;
}

.customer {
  font-size: 14px;
  line-height: 17px;
  color: #3c4257;
}

.date {
  font-size: 14px;
  line-height: 17px;
  color: #3c4257;
}
</style>