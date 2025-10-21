import React from "react";

export default function ZhoubaoFupan() {
  const sections = [
    {
      title: "😆 October Aim",
      items: [
        "AI generate fronted",
        "Zhihu title-drawer"
      ]
    },
    {
      title: "多动脑子",
      items: [
        "游戏的逻辑更简单可以思考得出，如技能、数值、走位动作",
        "输入习惯：成果up的早期高播放（后期同质化），知识点的开头部分",
        "业内人士怎么管理仓库",
        "从业人士讨论用法的可遇不可求：让工具更好用"
      ]
    },
    {
      title: "数学求知",
      items: [
        "裂项求项，无穷级数"
      ]
    },
    {
      title: "游戏求知",
      items: [
        "怪物图鉴"
      ]
    },
    {
      title: "娱乐部分",
      items: [
        "体育明星",
        "硬核文学"
      ]
    },
    {
      title: "渐进负重",
      items: [
        "咖啡",
        "会用AWS",
        "会用GPT问问题"
      ]
    },
    {
      title: "看不懂",
      items: [
        "技能点够多，认知能力，最后真的就走的远吗",
        "过去了，高格局有什么帮助？",
        "不安与现状的人，安于现状也还可以，但是？"
      ]
    }
  ];

  return (
    <div className="min-h-screen bg-neutral-950 text-neutral-100 p-8 flex flex-col items-center">
      <h1 className="text-4xl font-bold mb-6 text-teal-400"># zhoubaofupan</h1>
      <div className="max-w-3xl w-full grid gap-6">
        {sections.map((sec) => (
          <div key={sec.title} className="bg-neutral-900 rounded-2xl p-6 shadow-lg border border-neutral-800">
            <h2 className="text-2xl font-semibold mb-3 text-teal-300">{sec.title}</h2>
            <ul className="list-disc list-inside space-y-1 text-neutral-300">
              {sec.items.map((item, idx) => (
                <li key={idx}>{item}</li>
              ))}
            </ul>
          </div>
        ))}
      </div>
      <footer className="mt-10 text-neutral-600 text-sm">Designed by zhoubao · AI-assisted growth journal</footer>
    </div>
  );
}


